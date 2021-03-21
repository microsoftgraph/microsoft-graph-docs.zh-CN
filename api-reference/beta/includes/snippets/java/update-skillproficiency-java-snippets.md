---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f4e8b8f5ca13910201bc5203d10bfb5a8f3353c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968842"
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