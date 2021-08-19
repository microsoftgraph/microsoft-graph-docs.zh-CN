---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 990047e35efc04b6c34c14c41ec0d64683ccd8dfa68333b245c8ba46899085ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104798"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSubmission educationSubmission = graphClient.education().classes("11010").assignments("19002").submissions("33223")
    .buildRequest()
    .get();

```