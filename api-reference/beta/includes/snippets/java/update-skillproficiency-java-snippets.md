---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bbc0e2adb9767db562ee19ada3b321641e9fcc9767ebf480362a0737cd0c8d0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333319"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SkillProficiency skillProficiency = new SkillProficiency();
LinkedList<String> categoriesList = new LinkedList<String>();
categoriesList.add("Professional");
skillProficiency.categories = categoriesList;
skillProficiency.proficiency = SkillProficiencyLevel.ADVANCED_PROFESSIONAL;

graphClient.me().profile().skills("{id}")
    .buildRequest()
    .patch(skillProficiency);

```