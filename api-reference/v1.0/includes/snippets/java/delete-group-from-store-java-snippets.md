---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb85b7a28978a9336b238046fb0be8be32d7659d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109790"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74").termStore().groups("03577abb-975e-4fb4-9ee0-4102a9108f94")
    .buildRequest()
    .delete();

```