---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e3c453fcc649d9416da16520dec85fd5a81feb5995c80b65c3cfa052f7637cc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161881"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentResourceCollectionPage resources = graphClient.education().classes("11012").assignments("19002").resources()
    .buildRequest()
    .get();

```