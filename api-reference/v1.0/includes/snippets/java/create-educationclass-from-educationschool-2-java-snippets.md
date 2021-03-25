---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: afddc75fd5f077adca7f4c7bf63b4ab2b6bcc2ff
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211063"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("{class-id}").teachers("{teacher-id}")
    .buildRequest()
    .delete();

```