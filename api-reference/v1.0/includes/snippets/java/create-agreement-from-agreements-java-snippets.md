---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb6e62319c53ab6e4138db56abb471226c1d107e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774971"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Agreement agreement = new Agreement();
agreement.displayName = "MSGraph Sample";
agreement.isViewingBeforeAcceptanceRequired = true;
LinkedList<AgreementFileLocalization> filesList = new LinkedList<AgreementFileLocalization>();
AgreementFileLocalization files = new AgreementFileLocalization();
files.fileName = "TOU.pdf";
files.language = "en";
files.isDefault = true;
AgreementFileData fileData = new AgreementFileData();
fileData.data = Base64.getDecoder().decode("SGVsbG8gd29ybGQ=");
files.fileData = fileData;
filesList.add(files);
AgreementFileLocalizationCollectionResponse agreementFileLocalizationCollectionResponse = new AgreementFileLocalizationCollectionResponse();
agreementFileLocalizationCollectionResponse.value = filesList;
AgreementFileLocalizationCollectionPage agreementFileLocalizationCollectionPage = new AgreementFileLocalizationCollectionPage(agreementFileLocalizationCollectionResponse, null);
agreement.files = agreementFileLocalizationCollectionPage;

graphClient.identityGovernance().termsOfUse().agreements()
    .buildRequest()
    .post(agreement);

```