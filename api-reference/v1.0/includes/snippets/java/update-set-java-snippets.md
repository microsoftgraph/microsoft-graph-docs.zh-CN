---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7816e53def64a386a73e8a1f4b4f96c458b2faff
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084767"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Set set = new Set();
set.description = "mySet";

graphClient.sites("microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74").termStore().sets("3607e9f9-e9f9-3607-f9e9-0736f9e90736")
    .buildRequest()
    .patch(set);

```