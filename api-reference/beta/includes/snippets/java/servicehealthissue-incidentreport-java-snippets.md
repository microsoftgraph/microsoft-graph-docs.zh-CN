---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 207430f531676bf63db3b8cb076255cf9e5ddc0c8f96e382700806218b4c34dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105978"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.admin().serviceAnnouncement().issues("MO248163")
    .incidentReport()
    .buildRequest()
    .get();

```