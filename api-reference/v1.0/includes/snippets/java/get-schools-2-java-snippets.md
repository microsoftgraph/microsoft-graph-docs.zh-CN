---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c145b64ce1c9e75608540426a40d475a6580b4b
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210439"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchoolCollectionPage schools = graphClient.education().schools()
    .buildRequest()
    .get();

```