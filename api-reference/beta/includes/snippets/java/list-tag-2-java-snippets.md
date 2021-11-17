---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab7c918ce4128ba1cd3d0868cdf0dcce6bc73ae3d670f6913429187d7740fe21
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220303"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TagCollectionWithReferencesPage childTags = graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").tags("e54b3f535b434a9a8743b84e34c00504").childTags()
    .buildRequest()
    .get();

```