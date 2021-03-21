---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f1bd99f1715c6d9efc8147e9225f4c9e46f9e6a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967539"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Place place = graphClient.places("bldg1@contoso.com")
    .buildRequest()
    .get();

```