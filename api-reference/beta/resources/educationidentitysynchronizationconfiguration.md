---
title: educationIdentitySynchronizationConfiguration 资源类型
description: 所有学校数据配置文件标识同步配置的摘要基类。 派生类定义用于同步标识的行为。 以下是派生类型。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e282a9701eaae04aae33d9fd9efc9b86f7df3635
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972675"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="e9f07-105">educationIdentitySynchronizationConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9f07-105">educationIdentitySynchronizationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9f07-106">所有学校数据配置文件标识同步配置的摘要基类。</span><span class="sxs-lookup"><span data-stu-id="e9f07-106">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="e9f07-107">派生类定义用于同步标识的行为。</span><span class="sxs-lookup"><span data-stu-id="e9f07-107">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="e9f07-108">以下是派生类型。</span><span class="sxs-lookup"><span data-stu-id="e9f07-108">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="e9f07-109">派生类型</span><span class="sxs-lookup"><span data-stu-id="e9f07-109">Derived types</span></span>
| <span data-ttu-id="e9f07-110">类型</span><span class="sxs-lookup"><span data-stu-id="e9f07-110">Type</span></span> | <span data-ttu-id="e9f07-111">说明</span><span class="sxs-lookup"><span data-stu-id="e9f07-111">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="e9f07-112">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="e9f07-112">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="e9f07-113">使用此类型可匹配 Azure Active Directory (Azure AD) 中的现有用户帐户。</span><span class="sxs-lookup"><span data-stu-id="e9f07-113">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="e9f07-114">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="e9f07-114">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="e9f07-115">使用此类型在 Azure AD 中创建新用户帐户。</span><span class="sxs-lookup"><span data-stu-id="e9f07-115">Use this type to create new user accounts in Azure AD.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e9f07-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9f07-116">JSON representation</span></span>
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

