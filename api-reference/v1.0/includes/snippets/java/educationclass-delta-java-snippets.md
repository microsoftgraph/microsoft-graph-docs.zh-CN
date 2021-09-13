---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eea3d4e7bbc85a6e396770709edc5206f35b31490557369d7c46eb689fc37fb9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161625"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClassDeltaCollectionPage delta = graphClient.education().classes()
    .delta()
    .buildRequest()
    .get();

```