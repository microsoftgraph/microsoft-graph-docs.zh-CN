---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebd6fbaf938bd6f3de3db1335c6168703206c09c
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209615"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11014").assignments("19002")
    .buildRequest()
    .delete();

```