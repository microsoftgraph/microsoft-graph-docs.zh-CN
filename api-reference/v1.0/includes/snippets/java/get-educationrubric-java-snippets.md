---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a2774b017faefe1339a5a0a31990285e3abe729156faa79eceae1ae1c1288ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332791"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationRubric educationRubric = graphClient.education().me().rubrics("ceb3863e-6912-4ea9-ac41-3c2bb7b6672d")
    .buildRequest()
    .get();

```