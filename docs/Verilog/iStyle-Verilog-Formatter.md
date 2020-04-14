iStyle 项目地址：https://github.com/thomasrussellmurphy/istyle-verilog-formatter

VSCode 插件 verilog-formatter 地址：[Marketplace](https://marketplace.visualstudio.com/items?itemName=IsaacT.verilog-formatter) [GitHub](https://github.com/IsaacJT/Verilog-Formatter)

## Features

- 需编译 iStyle，或者可以直接下载[数逻实验/tools/iStyle.exe](https://github.com/duskmoon314/THU_EXP/blob/master/%E6%95%B0%E9%80%BB%E5%AE%9E%E9%AA%8C/tools/iStyle.exe)
  > 编译对于 win 存在一些困难，可以使用 wsl 等使用 Linux 的 make 进行编译
- 可配置使用 ANSI、GNU、K&R 三种代码风格，也可以添加 args 进行些微的修改
- 对单文件多`module`的缩进效果一般

## 效果

待格式化代码

```verilog
reg [3:0] cnt;
always @(posedge clk or posedge rst) begin
if(rst) begin
cnt<=4'h0;
end else begin
cnt<=cnt+4'h1;
end
end
```

**--style**

ANSI style

`./iStyle --style=ansi test.v`

```verilog
reg [3:0] cnt;
always @(posedge clk or posedge rst)
begin
    if(rst)
    begin
        cnt<=4'h0;
    end
    else
    begin
        cnt<=cnt+4'h1;
    end
end
```

Kernighan&Ritchie style

`./iStyle --style=kr test.v`

```verilog
reg [3:0] cnt;
always @(posedge clk or posedge rst) begin
    if(rst) begin
        cnt<=4'h0;
    end
    else begin
        cnt<=cnt+4'h1;
    end
end
```

GNU style

`./iStyle --style=gnu test.v`

```verilog
reg [3:0] cnt;
always @(posedge clk or posedge rst)
  begin
    if(rst)
      begin
        cnt<=4'h0;
      end
    else
      begin
        cnt<=cnt+4'h1;
      end
  end
```
