---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60bbda3e15fcf804e9c9ce834ce1528703495385
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980338"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProfileCardProperty profileCardProperty = new ProfileCardProperty();
LinkedList<ProfileCardAnnotation> annotationsList = new LinkedList<ProfileCardAnnotation>();
ProfileCardAnnotation annotations = new ProfileCardAnnotation();
LinkedList<DisplayNameLocalization> localizationsList = new LinkedList<DisplayNameLocalization>();
DisplayNameLocalization localizations = new DisplayNameLocalization();
localizations.languageTag = "no-NB";
localizations.displayName = "Kostnads Senter";
localizationsList.add(localizations);
annotations.localizations = localizationsList;
annotationsList.add(annotations);
profileCardProperty.annotations = annotationsList;

graphClient.organization("{organizationId}").settings().profileCardProperties("CustomAttribute1")
    .buildRequest()
    .patch(profileCardProperty);

```