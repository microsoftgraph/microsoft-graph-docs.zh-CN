---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3d99724cb0bd59873cf80e4dd326e540c544c6f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977847"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExtensionPropertyCollectionPage extensionProperties = graphClient.applications("{id}").extensionProperties()
    .buildRequest()
    .get();

```