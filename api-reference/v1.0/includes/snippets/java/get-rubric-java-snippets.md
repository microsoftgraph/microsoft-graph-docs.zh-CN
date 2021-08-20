---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93b0519f2b23163c24516c951b33f57341b013a2855d6898c243c09840bb2ffb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277184"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationRubric educationRubric = graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments("cf6005fc-9e13-44a2-a6ac-a53322006454").rubric()
    .buildRequest()
    .get();

```