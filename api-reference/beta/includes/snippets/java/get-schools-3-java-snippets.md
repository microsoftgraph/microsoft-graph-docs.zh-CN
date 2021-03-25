---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93d8c21c433c9322a8e362d834d1333d180efbfd
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211181"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchoolCollectionWithReferencesPage schools = graphClient.education().me().schools()
    .buildRequest()
    .get();

```