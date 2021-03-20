---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 118cec549a464276526e890d7989b3706927d40c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968187"
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