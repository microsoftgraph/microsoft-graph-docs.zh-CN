---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af5fd662a232b6b868903c7518729bb7a2bfc085
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979571"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProjectParticipation projectParticipation = new ProjectParticipation();
LinkedList<String> categoriesList = new LinkedList<String>();
categoriesList.add("Branding");
projectParticipation.categories = categoriesList;
CompanyDetail client = new CompanyDetail();
client.displayName = "Contoso Ltd.";
client.department = "Corporate Marketing";
client.webUrl = "https://www.contoso.com";
projectParticipation.client = client;
projectParticipation.displayName = "Contoso Re-branding Project";
PositionDetail detail = new PositionDetail();
CompanyDetail company = new CompanyDetail();
company.displayName = "Adventureworks Inc.";
company.department = "Consulting";
company.webUrl = "https://adventureworks.com";
detail.company = company;
detail.description = "Rebranding of Contoso Ltd.";
detail.jobTitle = "Lead PM Rebranding";
detail.role = "project management";
detail.summary = "A 6 month project to help Contoso rebrand after they were divested from a parent organization.";
projectParticipation.detail = detail;

graphClient.me().profile().projects()
    .buildRequest()
    .post(projectParticipation);

```