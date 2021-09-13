---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79dfc00628003274ec5d066d2fb8cffc11e2214f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094638"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Term term = graphClient.sites("microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74").termStore().groups("8401c566-a86e-4734-a4db-eeb434cd99f9").sets("dcaae29d-2234-4619-bccf-c2ec50b52344").terms("81be9856-9856-81be-5698-be815698be81")
    .buildRequest()
    .get();

```