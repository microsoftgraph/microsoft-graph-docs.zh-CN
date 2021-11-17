---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4970435ec400669d9d2b240d5c14d93e31ba47f6c89a17a16df8cedbdc9f9af7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903753"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProfileCardProperty profileCardProperty = graphClient.organization("{organizationId}").settings().profileCardProperties("{id}")
    .buildRequest()
    .get();

```