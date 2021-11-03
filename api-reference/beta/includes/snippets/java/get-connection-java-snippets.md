---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4aab039d4f19334e01e0e66dcb72f6bf271f57e2
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696150"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalConnection externalConnection = graphClient.external().connections("contosohr")
    .buildRequest()
    .get();

```