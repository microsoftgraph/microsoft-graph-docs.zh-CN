---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6db91f5b3f73337ac5e81e40a5df9529bc63af27
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956586"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().schools("{school-id}").users("{user-id}")
    .buildRequest()
    .delete();

```