---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29daf462a93912dcb61b4c16e56595f20cd259a6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959233"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Fido2AuthenticationMethod fido2AuthenticationMethod = graphClient.me().authentication().fido2Methods("-2_GRUg2-HYz6_1YG4YRAQ2")
    .buildRequest()
    .get();

```