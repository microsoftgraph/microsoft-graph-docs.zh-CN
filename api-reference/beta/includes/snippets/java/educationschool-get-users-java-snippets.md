---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d3194e746792311eb5fdde83ec3d0933123d766e5afdd08c7ded4b9e9a87168
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273898"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUserCollectionWithReferencesPage users = graphClient.education().schools("10002").users()
    .buildRequest()
    .get();

```