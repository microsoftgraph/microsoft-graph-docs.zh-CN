---
title: educationIdentitySynchronizationConfiguration 资源类型
description: 所有学校数据配置文件标识同步配置的抽象基类。 派生的类定义同步标识的行为。 以下是派生的类型。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 59dca28f82de0340aa289c6ea96ef5e252f60e85
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412903"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="04ea5-105">educationIdentitySynchronizationConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="04ea5-105">educationIdentitySynchronizationConfiguration resource type</span></span>

> <span data-ttu-id="04ea5-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="04ea5-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04ea5-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="04ea5-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="04ea5-108">所有学校数据配置文件标识同步配置的抽象基类。</span><span class="sxs-lookup"><span data-stu-id="04ea5-108">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="04ea5-109">派生的类定义同步标识的行为。</span><span class="sxs-lookup"><span data-stu-id="04ea5-109">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="04ea5-110">以下是派生的类型。</span><span class="sxs-lookup"><span data-stu-id="04ea5-110">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="04ea5-111">派生的类型</span><span class="sxs-lookup"><span data-stu-id="04ea5-111">Derived types</span></span>
| <span data-ttu-id="04ea5-112">类型</span><span class="sxs-lookup"><span data-stu-id="04ea5-112">Type</span></span> | <span data-ttu-id="04ea5-113">说明</span><span class="sxs-lookup"><span data-stu-id="04ea5-113">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="04ea5-114">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="04ea5-114">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="04ea5-115">使用此类型来匹配 Azure Active Directory (Azure AD) 中的现有用户帐户。</span><span class="sxs-lookup"><span data-stu-id="04ea5-115">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="04ea5-116">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="04ea5-116">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="04ea5-117">使用此类型在 Azure AD 中创建新的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="04ea5-117">Use this type to create new user accounts in Azure AD.</span></span> |

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{
}
```
