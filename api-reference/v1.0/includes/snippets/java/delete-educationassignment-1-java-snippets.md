---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c8fa103247a5bd34dd7990ec73449d691a02f1894bc888b9df06069e8e92bf0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107052"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("c42f493f-42b4-4e7d-8148-af894cbc518b").assignments("ad8afb28-c138-4ad7-b7f5-a6986c2655a8")
    .buildRequest()
    .delete();

```