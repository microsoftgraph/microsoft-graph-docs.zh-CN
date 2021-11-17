---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d64cf510ba9ed695b8e77398332d5011150b1aa1f1d4ffb9a72f6f3fcbe6ae18
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277983"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Set set = graphClient.sites("microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f").termStore().sets("8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f")
    .buildRequest()
    .get();

```