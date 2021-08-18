---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 636d87caade70b46b520df63bcc726608717331444391ba1350d28253f147bb8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163992"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSubmissionResourceCollectionPage resources = graphClient.education().classes("{id}").assignments("{id}").submissions("{id}").resources()
    .buildRequest()
    .get();

```