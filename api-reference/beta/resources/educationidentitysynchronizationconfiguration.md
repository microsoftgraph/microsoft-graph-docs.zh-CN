---
title: educationIdentitySynchronizationConfiguration 资源类型
description: 所有学校数据配置文件标识同步配置的摘要基类。 派生类定义用于同步标识的行为。 以下是派生类型。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1ffa1bbcd3f96c86818c68d350236086d0975187
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501792"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="bc9f4-105">educationIdentitySynchronizationConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc9f4-105">educationIdentitySynchronizationConfiguration resource type</span></span>

<span data-ttu-id="bc9f4-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="bc9f4-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc9f4-107">所有学校数据配置文件标识同步配置的摘要基类。</span><span class="sxs-lookup"><span data-stu-id="bc9f4-107">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="bc9f4-108">派生类定义用于同步标识的行为。</span><span class="sxs-lookup"><span data-stu-id="bc9f4-108">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="bc9f4-109">以下是派生类型。</span><span class="sxs-lookup"><span data-stu-id="bc9f4-109">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="bc9f4-110">派生类型</span><span class="sxs-lookup"><span data-stu-id="bc9f4-110">Derived types</span></span>
| <span data-ttu-id="bc9f4-111">类型</span><span class="sxs-lookup"><span data-stu-id="bc9f4-111">Type</span></span> | <span data-ttu-id="bc9f4-112">说明</span><span class="sxs-lookup"><span data-stu-id="bc9f4-112">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="bc9f4-113">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="bc9f4-113">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="bc9f4-114">使用此类型可匹配 Azure Active Directory （Azure AD）中的现有用户帐户。</span><span class="sxs-lookup"><span data-stu-id="bc9f4-114">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="bc9f4-115">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="bc9f4-115">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="bc9f4-116">使用此类型在 Azure AD 中创建新用户帐户。</span><span class="sxs-lookup"><span data-stu-id="bc9f4-116">Use this type to create new user accounts in Azure AD.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bc9f4-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc9f4-117">JSON representation</span></span>
<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{
}
```

