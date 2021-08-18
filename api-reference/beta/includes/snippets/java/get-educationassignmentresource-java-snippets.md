---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 221ea996f045c4dce53db59070936d605cae3ff3ea9dc20ecdf25720d5c5cc97
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219148"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentResource educationAssignmentResource = graphClient.education().classes("11021").assignments("19002").resources("22002")
    .buildRequest()
    .get();

```