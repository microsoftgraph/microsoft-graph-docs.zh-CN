---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91e8981270ddf0b83a25feed5fd7a1cb292c49ea7ccdb3360cbc9a7a73429a2d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105554"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProfileCardProperty profileCardProperty = new ProfileCardProperty();
profileCardProperty.directoryPropertyName = "CustomAttribute1";
LinkedList<ProfileCardAnnotation> annotationsList = new LinkedList<ProfileCardAnnotation>();
ProfileCardAnnotation annotations = new ProfileCardAnnotation();
annotations.displayName = "Cost Center";
LinkedList<DisplayNameLocalization> localizationsList = new LinkedList<DisplayNameLocalization>();
DisplayNameLocalization localizations = new DisplayNameLocalization();
localizations.languageTag = "ru-RU";
localizations.displayName = "центр затрат";
localizationsList.add(localizations);
annotations.localizations = localizationsList;
annotationsList.add(annotations);
profileCardProperty.annotations = annotationsList;

graphClient.organization("{organizationId}").settings().profileCardProperties()
    .buildRequest()
    .post(profileCardProperty);

```