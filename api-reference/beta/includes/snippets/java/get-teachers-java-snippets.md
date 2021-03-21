---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61bbb4a2041b99f7eb7836c2fe9d27dbd8adc651
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982872"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUserCollectionWithReferencesPage teachers = graphClient.education().classes("11023").teachers()
    .buildRequest()
    .get();

```