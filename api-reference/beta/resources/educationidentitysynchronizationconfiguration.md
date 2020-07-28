---
title: educationIdentitySynchronizationConfiguration 资源类型
description: 所有学校数据配置文件标识同步配置的摘要基类。 派生类定义用于同步标识的行为。 以下是派生类型。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1c3531999065abc22cc0ecb1870b4bd1bb5f45b7
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435017"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="16e4f-105">educationIdentitySynchronizationConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="16e4f-105">educationIdentitySynchronizationConfiguration resource type</span></span>

<span data-ttu-id="16e4f-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16e4f-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16e4f-107">所有学校数据配置文件标识同步配置的摘要基类。</span><span class="sxs-lookup"><span data-stu-id="16e4f-107">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="16e4f-108">派生类定义用于同步标识的行为。</span><span class="sxs-lookup"><span data-stu-id="16e4f-108">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="16e4f-109">以下是派生类型。</span><span class="sxs-lookup"><span data-stu-id="16e4f-109">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="16e4f-110">派生类型</span><span class="sxs-lookup"><span data-stu-id="16e4f-110">Derived types</span></span>

| <span data-ttu-id="16e4f-111">类型</span><span class="sxs-lookup"><span data-stu-id="16e4f-111">Type</span></span>                                                                                | <span data-ttu-id="16e4f-112">说明</span><span class="sxs-lookup"><span data-stu-id="16e4f-112">Description</span></span>                                                                         |
| :---------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------- |
| [<span data-ttu-id="16e4f-113">educationIdentityMatchingConfiguration</span><span class="sxs-lookup"><span data-stu-id="16e4f-113">educationIdentityMatchingConfiguration</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="16e4f-114">使用此类型可**匹配**Azure Active Directory 中的现有用户帐户。</span><span class="sxs-lookup"><span data-stu-id="16e4f-114">Use this type to **match existing** user accounts in Azure Active Directory.</span></span> |
| [<span data-ttu-id="16e4f-115">educationIdentityCreationConfiguration</span><span class="sxs-lookup"><span data-stu-id="16e4f-115">educationIdentityCreationConfiguration</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="16e4f-116">使用此类型在 Azure Active Directory 中**创建新**用户帐户。</span><span class="sxs-lookup"><span data-stu-id="16e4f-116">Use this type to **create new** user accounts in Azure Active Directory.</span></span>                              |

## <a name="json-representation"></a><span data-ttu-id="16e4f-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16e4f-117">JSON representation</span></span>

<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{}
```
