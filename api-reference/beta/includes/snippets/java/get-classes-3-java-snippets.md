---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27e53e5e211e3630c84bd7fdb5010ae7d9588219835acf153365088edafe6e04
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161266"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClassCollectionWithReferencesPage classes = graphClient.education().me().classes()
    .buildRequest()
    .get();

```