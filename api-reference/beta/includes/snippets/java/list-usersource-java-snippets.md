---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7733cc5f6eeeb7bfcc9a719d3e9a12c3cae5a94aa145e3ac2fdf8ae381d238d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219251"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserSourceCollectionPage userSources = graphClient.compliance().ediscovery().cases("c816dd6f-5af8-40c5-a760-331361e05c60").legalHolds("277107ff-fee3-41a0-a665-a9d7f6c4824f").userSources()
    .buildRequest()
    .get();

```