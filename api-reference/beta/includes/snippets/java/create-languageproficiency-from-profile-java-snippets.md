---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d43855f0a86d355a6719b6c574c0cbf1a8937bed25392115ef80567467e2cbd7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220857"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LanguageProficiency languageProficiency = new LanguageProficiency();
languageProficiency.displayName = "Norwegian Bokmål";
languageProficiency.tag = "nb-NO";
languageProficiency.spoken = LanguageProficiencyLevel.NATIVE_OR_BILINGUAL;
languageProficiency.written = LanguageProficiencyLevel.NATIVE_OR_BILINGUAL;
languageProficiency.reading = LanguageProficiencyLevel.NATIVE_OR_BILINGUAL;

graphClient.me().profile().languages()
    .buildRequest()
    .post(languageProficiency);

```