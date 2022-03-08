---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88617593d39211c84531015e34b0e645850c2e0a
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854274"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceRequest accessPackageResourceRequest = new AccessPackageResourceRequest();
accessPackageResourceRequest.catalogId = "26ac0c0a-08bc-4a7b-a313-839f58044ba5";
accessPackageResourceRequest.requestType = "AdminAdd";
accessPackageResourceRequest.justification = "";
AccessPackageResource accessPackageResource = new AccessPackageResource();
accessPackageResource.displayName = "Faculty cafeteria ordering";
accessPackageResource.description = "Example application";
accessPackageResource.url = "https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/";
accessPackageResource.resourceType = "Application";
accessPackageResource.originId = "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e";
accessPackageResource.originSystem = "AadApplication";
LinkedList<AccessPackageResourceAttribute> attributesList = new LinkedList<AccessPackageResourceAttribute>();
AccessPackageResourceAttribute attributes = new AccessPackageResourceAttribute();
attributes.attributeName = "extension_2b676109c7c74ae2b41549205f1947ed_personalTitle";
attributes.isEditable = true;
attributes.isPersistedOnAssignmentRemoval = true;
AccessPackageResourceAttributeQuestion attributeSource = new AccessPackageResourceAttributeQuestion();
AccessPackageTextInputQuestion question = new AccessPackageTextInputQuestion();
question.isRequired = false;
question.sequence = 0;
question.isSingleLineQuestion = true;
AccessPackageLocalizedContent text = new AccessPackageLocalizedContent();
text.defaultText = "Title";
LinkedList<AccessPackageLocalizedText> localizedTextsList = new LinkedList<AccessPackageLocalizedText>();
text.localizedTexts = localizedTextsList;
question.text = text;
attributeSource.question = question;
attributes.attributeSource = attributeSource;
AccessPackageUserDirectoryAttributeStore attributeDestination = new AccessPackageUserDirectoryAttributeStore();
attributes.attributeDestination = attributeDestination;
attributesList.add(attributes);
accessPackageResource.attributes = attributesList;
accessPackageResourceRequest.accessPackageResource = accessPackageResource;

graphClient.identityGovernance().entitlementManagement().accessPackageResourceRequests()
    .buildRequest()
    .post(accessPackageResourceRequest);

```