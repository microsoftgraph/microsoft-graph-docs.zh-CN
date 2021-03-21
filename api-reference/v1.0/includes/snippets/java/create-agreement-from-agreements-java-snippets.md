---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98c7f79a462950ebfdf49779b14080a890f69e75
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981810"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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