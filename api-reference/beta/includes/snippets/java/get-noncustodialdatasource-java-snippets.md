---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4d0c328e538e442ec705ffb50090b236dab21362f7b9376dd2e08a0f5cb2a66
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103883"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NoncustodialDataSource noncustodialDataSource = graphClient.compliance().ediscovery().cases("5b840b94-f821-4c4a-8cad-3a90062bf51a").noncustodialDataSources("8b69818bf6af4f8a9dede428401c71e7")
    .buildRequest()
    .get();

```