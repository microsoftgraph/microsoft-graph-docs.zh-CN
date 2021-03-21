---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 690218a1193d2ed50db564c8c5c4116d23a93825
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972542"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookUserSupportedLanguagesCollectionPage supportedLanguages = graphClient.me().outlook()
    .supportedLanguages()
    .buildRequest()
    .get();

```