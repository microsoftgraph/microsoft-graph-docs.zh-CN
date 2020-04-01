---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e8d963748c5c05bdfa8fa79a1e96928a5e5b66f
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082149"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrgContact orgContact = graphClient.contacts("delta")
    .buildRequest()
    .select("displayName,jobTitle,mail")
    .get();

```