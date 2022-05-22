---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64daf6ff3616f25b7e708073864acbbe7c58dd78
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65628875"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AgreementFileLocalization agreementFileLocalization = new AgreementFileLocalization();
agreementFileLocalization.fileName = "Contoso ToU for guest users (French)";
agreementFileLocalization.language = "fr-FR";
agreementFileLocalization.isDefault = false;
agreementFileLocalization.isMajorVersion = false;
agreementFileLocalization.displayName = "Contoso ToU for guest users (French)";
AgreementFileData fileData = new AgreementFileData();
fileData.data = Base64.getDecoder().decode("base64JVBERi0xLjUKJb/3ov4KNCAwIG9iago8PCAvTGluZWFyaX//truncated-binary-data");
agreementFileLocalization.fileData = fileData;

graphClient.identityGovernance().termsOfUse().agreements("94410bbf-3d3e-4683-8149-f034e55c39dd").files()
    .buildRequest()
    .post(agreementFileLocalization);

```