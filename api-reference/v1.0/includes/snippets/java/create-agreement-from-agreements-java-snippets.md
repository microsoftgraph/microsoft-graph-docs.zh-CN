---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7963e5fe274b7bc6bb8c01e925cda1e394b6e20231c51179318df4a57aa1296e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333283"
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