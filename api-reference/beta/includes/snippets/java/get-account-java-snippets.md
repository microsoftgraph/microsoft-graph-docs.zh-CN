---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0adfdb2cea484c20b171c03af32f205957a90b47
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978194"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserAccountInformationCollectionPage account = graphClient.me().profile().account()
    .buildRequest()
    .get();

```