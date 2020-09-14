# Directive

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 8.3.22.

## introduction

This project is a trainning about create an introduce like *ng-For by myself

该项目是一个关于创建自定义结构型指令的训练

## The way to create 

1.首先创建一个appIf.directice.ts文件，通过@input以传值的方式将appIf传进来，并通过判断它的判断它的布尔值对组件进行显示或隐藏。

2.响应用户操作
  （1）首先需要在app.module.ts中注入指令。
       import { AppIfDirective } from './appIf.directive';
       declarations: [AppComponent,AppIfDirective],
  （2）接下来在app.component.html构建用于展示内容的页面
  （3）最后在app.component.ts完成方法
       changeShow(sex: string) {
          if (sex === 'man') {
              this.isMan = true;
          } else {
              this.isMan = false;
          }
        }


## Development server

运行：

npm install

npm start

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`


