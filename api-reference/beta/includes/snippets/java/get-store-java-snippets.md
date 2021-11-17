---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a360e8917b4d2d6d0e9b24e1850eaf2b3578c515727f0d83c5344a19136a2404
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277969"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Store store = graphClient.sites("microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f").termStore()
    .buildRequest()
    .get();

```