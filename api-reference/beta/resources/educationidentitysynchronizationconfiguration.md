---
title: educationIdentitySynchronizationConfiguration 资源类型
description: 所有学校数据配置文件标识同步配置的摘要基类。 派生类定义用于同步标识的行为。 以下是派生类型。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 713bb285e739d9182a982f02975a9b9f46761e3a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736514"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="f1b96-105">educationIdentitySynchronizationConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1b96-105">educationIdentitySynchronizationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1b96-106">所有学校数据配置文件标识同步配置的摘要基类。</span><span class="sxs-lookup"><span data-stu-id="f1b96-106">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="f1b96-107">派生类定义用于同步标识的行为。</span><span class="sxs-lookup"><span data-stu-id="f1b96-107">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="f1b96-108">以下是派生类型。</span><span class="sxs-lookup"><span data-stu-id="f1b96-108">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="f1b96-109">派生类型</span><span class="sxs-lookup"><span data-stu-id="f1b96-109">Derived types</span></span>
| <span data-ttu-id="f1b96-110">类型</span><span class="sxs-lookup"><span data-stu-id="f1b96-110">Type</span></span> | <span data-ttu-id="f1b96-111">说明</span><span class="sxs-lookup"><span data-stu-id="f1b96-111">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="f1b96-112">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="f1b96-112">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="f1b96-113">使用此类型可匹配 Azure Active Directory (Azure AD) 中的现有用户帐户。</span><span class="sxs-lookup"><span data-stu-id="f1b96-113">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="f1b96-114">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="f1b96-114">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="f1b96-115">使用此类型在 Azure AD 中创建新用户帐户。</span><span class="sxs-lookup"><span data-stu-id="f1b96-115">Use this type to create new user accounts in Azure AD.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f1b96-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1b96-116">JSON representation</span></span>
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

