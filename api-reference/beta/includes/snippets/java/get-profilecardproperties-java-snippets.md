---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ac46a3592527214a21854c811d09d85fa3f17540916157e1fee276916a8e13d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273860"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProfileCardPropertyCollectionPage profileCardProperties = graphClient.organization("{organizationId}").settings().profileCardProperties()
    .buildRequest()
    .get();

```