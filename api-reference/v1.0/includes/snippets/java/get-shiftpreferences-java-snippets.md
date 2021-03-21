---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ed8fdc892763980669a4735be9f43ddcd6c3917
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968575"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ShiftPreferences shiftPreferences = graphClient.users("871dbd5c-3a6a-4392-bfe1-042452793a50").settings().shiftPreferences()
    .buildRequest()
    .get();

```