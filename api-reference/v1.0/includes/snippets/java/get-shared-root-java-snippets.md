---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab66b90da493e449a3fd1b4f7a3de13a9643b0b99a2546195401fcd3d8f13ca4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218664"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SharedDriveItem sharedDriveItem = graphClient.shares("{shareIdOrEncodedSharingUrl}")
    .buildRequest()
    .get();

```