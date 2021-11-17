---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a413b8b79187ee4ef01956e32dcaa49205e1a903a8d0ad70aece4bb3b14c4aa4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164097"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OpenShiftChangeRequest openShiftChangeRequest = graphClient.teams("{id}").schedule().openShiftChangeRequests("SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09")
    .buildRequest()
    .get();

```