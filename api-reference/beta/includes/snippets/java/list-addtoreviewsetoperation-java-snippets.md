---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f38c625f4fba2c88b4935166a4e2ae07183fc833c469b8a49043508d4f89d491
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162500"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AddToReviewSetOperation addToReviewSetOperation = graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").sourceCollections("1a9b4145d8f84e39bc45a7f68c5c5119").addToReviewSetOperation()
    .buildRequest()
    .get();

```