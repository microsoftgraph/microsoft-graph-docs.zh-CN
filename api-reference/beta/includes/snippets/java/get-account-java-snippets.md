---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ddb56f560c3bb4622a1ed1bb465312cb56238028
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772469"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserAccountInformationCollectionPage account = graphClient.me().profile().account()
    .buildRequest()
    .get();

```