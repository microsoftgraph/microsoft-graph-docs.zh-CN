---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf69afb6191ab6a42a4de7a78c591b851b1e24c59f2f1ef663100d69498fbd83
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278341"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSubmissionResource educationSubmissionResource = graphClient.education().classes("11021").assignments("19002").submissions("850f51b7").resources("f2387c3b-ec39-4bf2-a399-d7242677f024")
    .buildRequest()
    .get();

```