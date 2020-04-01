---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cbf6f788a5878bc4a1d45670c3d2c22169f7034
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082155"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrgContact orgContact = graphClient.contacts("delta")
    .buildRequest()
    .get();

```