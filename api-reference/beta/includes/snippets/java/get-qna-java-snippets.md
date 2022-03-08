---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ed0ab36db0264940eda710dfd780be2a56602ff
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338263"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Qna qna = graphClient.search().qnas("{qnaId}")
    .buildRequest()
    .get();

```