---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99496eeeb168bb37fdd18e32bcbb87ac2d180f4c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962442"
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

graphClient.agreements()
    .buildRequest()
    .post(agreement);

```