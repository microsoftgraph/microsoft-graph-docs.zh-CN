---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0f08840f8843f67e1fc3b22ba06a7338c2b36a9
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200899"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
LinkedList<RelatedContact> relatedContactsList = new LinkedList<RelatedContact>();
RelatedContact relatedContacts = new RelatedContact();
relatedContacts.displayName = "Father Time";
relatedContacts.emailAddress = "father@time.com";
relatedContacts.mobilePhone = "4251231234";
relatedContacts.relationship = ContactRelationship.GUARDIAN;
relatedContacts.accessConsent = true;
relatedContactsList.add(relatedContacts);
RelatedContact relatedContacts1 = new RelatedContact();
relatedContacts1.displayName = "Mother Nature";
relatedContacts1.emailAddress = "mother@nature.co.uk";
relatedContacts1.mobilePhone = "3251231234";
relatedContacts1.relationship = ContactRelationship.PARENT;
relatedContacts1.accessConsent = true;
relatedContactsList.add(relatedContacts1);
educationUser.relatedContacts = relatedContactsList;

graphClient.education().users("{educationUserId}")
    .buildRequest()
    .patch(educationUser);

```