---
title: educationIdentitySynchronizationConfiguration 资源类型
description: 所有学校数据配置文件标识同步配置的抽象基类。 派生的类定义同步标识的行为。 以下是派生的类型。
ms.openlocfilehash: 4476e3b50354fef024925823a8aa1b53ee5a5d3d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045714"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="6a6af-105">educationIdentitySynchronizationConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a6af-105">educationIdentitySynchronizationConfiguration resource type</span></span>

> <span data-ttu-id="6a6af-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6a6af-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a6af-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6a6af-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a6af-108">所有学校数据配置文件标识同步配置的抽象基类。</span><span class="sxs-lookup"><span data-stu-id="6a6af-108">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="6a6af-109">派生的类定义同步标识的行为。</span><span class="sxs-lookup"><span data-stu-id="6a6af-109">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="6a6af-110">以下是派生的类型。</span><span class="sxs-lookup"><span data-stu-id="6a6af-110">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="6a6af-111">派生的类型</span><span class="sxs-lookup"><span data-stu-id="6a6af-111">Derived types</span></span>
| <span data-ttu-id="6a6af-112">类型</span><span class="sxs-lookup"><span data-stu-id="6a6af-112">Type</span></span> | <span data-ttu-id="6a6af-113">说明</span><span class="sxs-lookup"><span data-stu-id="6a6af-113">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="6a6af-114">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="6a6af-114">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="6a6af-115">使用此类型来匹配 Azure Active Directory (Azure AD) 中的现有用户帐户。</span><span class="sxs-lookup"><span data-stu-id="6a6af-115">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="6a6af-116">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="6a6af-116">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="6a6af-117">使用此类型在 Azure AD 中创建新的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="6a6af-117">Use this type to create new user accounts in Azure AD.</span></span> |
