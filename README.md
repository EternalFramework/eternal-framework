
# 工程结构
```shell
eternal-framework
├── dependencies          # 统一依赖版本管理（BOM）
├── foundation            # 基础核心层（所有能力实现）
│   ├── core              # 无框架依赖的纯Java核心工具
│   │    └── eternal-core
│   ├── spring-boot       # Spring Boot 基础支撑（非Web）
│   │    ├── eternal-spring-boot
│   │    └── eternal-spring-boot-autoconfigure
│   └── web               # Web 全场景支撑（MVC + WebFlux）
│        ├── eternal-web        # Web 通用定义/常量/枚举
│        ├── eternal-webmvc
│        ├── eternal-webmvc-autoconfigure
│        ├── eternal-webflux
│        └── eternal-webflux-autoconfigure
├── parent                # 父POM（统一插件、仓库、构建）
└── starters               # 官方Starter（只引依赖，无代码）
     ├── eternal-spring-boot-starter
     ├── eternal-cloud-spring-boot-starter
     ├── eternal-webmvc-spring-boot-starter
     └── eternal-webflux-spring-boot-starter
```