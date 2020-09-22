---
title: educationIdentitySynchronizationConfiguration 资源类型
description: 所有学校数据配置文件标识同步配置的摘要基类。 派生类定义用于同步标识的行为。 以下是派生类型。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8e193c798f1f3fbc5d4d1c9d8c7b96eed7d39cf9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095357"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="7f2fc-105">educationIdentitySynchronizationConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f2fc-105">educationIdentitySynchronizationConfiguration resource type</span></span>

<span data-ttu-id="7f2fc-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f2fc-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f2fc-107">所有学校数据配置文件标识同步配置的摘要基类。</span><span class="sxs-lookup"><span data-stu-id="7f2fc-107">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="7f2fc-108">派生类定义用于同步标识的行为。</span><span class="sxs-lookup"><span data-stu-id="7f2fc-108">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="7f2fc-109">以下是派生类型。</span><span class="sxs-lookup"><span data-stu-id="7f2fc-109">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="7f2fc-110">派生类型</span><span class="sxs-lookup"><span data-stu-id="7f2fc-110">Derived types</span></span>

| <span data-ttu-id="7f2fc-111">类型</span><span class="sxs-lookup"><span data-stu-id="7f2fc-111">Type</span></span>                                                                                | <span data-ttu-id="7f2fc-112">说明</span><span class="sxs-lookup"><span data-stu-id="7f2fc-112">Description</span></span>                                                                         |
| :---------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------- |
| [<span data-ttu-id="7f2fc-113">educationIdentityMatchingConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f2fc-113">educationIdentityMatchingConfiguration</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="7f2fc-114">使用此类型可 **匹配** Azure Active Directory 中的现有用户帐户。</span><span class="sxs-lookup"><span data-stu-id="7f2fc-114">Use this type to **match existing** user accounts in Azure Active Directory.</span></span> |
| [<span data-ttu-id="7f2fc-115">educationIdentityCreationConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f2fc-115">educationIdentityCreationConfiguration</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="7f2fc-116">使用此类型在 Azure Active Directory 中 **创建新** 用户帐户。</span><span class="sxs-lookup"><span data-stu-id="7f2fc-116">Use this type to **create new** user accounts in Azure Active Directory.</span></span>                              |

## <a name="json-representation"></a><span data-ttu-id="7f2fc-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f2fc-117">JSON representation</span></span>

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


