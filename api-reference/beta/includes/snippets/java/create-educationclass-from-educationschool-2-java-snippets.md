---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80cbfdf61cdcdc366739def53a37f9e7de731ff9
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210770"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("{id}").teachers("14012")
    .buildRequest()
    .delete();

```