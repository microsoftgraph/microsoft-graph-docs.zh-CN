---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4430fe2a79bc167fd925a82ede7ccff881fe920f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855456"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Agreement agreement = new Agreement();
agreement.displayName = "MSGraph Sample";
agreement.isViewingBeforeAcceptanceRequired = true;
LinkedList<AgreementFile> filesList = new LinkedList<AgreementFile>();
AgreementFile files = new AgreementFile();
files.fileName = "TOU.pdf";
files.language = "en";
files.isDefault = true;
AgreementFileData fileData = new AgreementFileData();
fileData.data = "SGVsbG8gd29ybGQ=";
files.fileData = fileData;
filesList.add(files);
agreement.files = filesList;

graphClient.agreements()
    .buildRequest()
    .post(agreement);

```