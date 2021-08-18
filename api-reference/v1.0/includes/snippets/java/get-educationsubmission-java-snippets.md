---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30d88471d9644fd0be4944305df715c6536f6a44fad2ac5f652a86101c8bbb15
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409061"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSubmission educationSubmission = graphClient.education().classes("11010").assignments("ad8afb28-c138-4ad7-b7f5-a6986c2655a8").submissions("33223")
    .buildRequest()
    .get();

```