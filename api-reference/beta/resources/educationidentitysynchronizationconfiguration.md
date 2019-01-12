---
title: educationIdentitySynchronizationConfiguration 资源类型
description: 所有学校数据配置文件标识同步配置的抽象基类。 派生的类定义同步标识的行为。 以下是派生的类型。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 6d9841d4957d5330fc966f60a24582e101831b6c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969028"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="a8fd0-105">educationIdentitySynchronizationConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8fd0-105">educationIdentitySynchronizationConfiguration resource type</span></span>

> <span data-ttu-id="a8fd0-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a8fd0-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8fd0-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a8fd0-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8fd0-108">所有学校数据配置文件标识同步配置的抽象基类。</span><span class="sxs-lookup"><span data-stu-id="a8fd0-108">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="a8fd0-109">派生的类定义同步标识的行为。</span><span class="sxs-lookup"><span data-stu-id="a8fd0-109">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="a8fd0-110">以下是派生的类型。</span><span class="sxs-lookup"><span data-stu-id="a8fd0-110">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="a8fd0-111">派生的类型</span><span class="sxs-lookup"><span data-stu-id="a8fd0-111">Derived types</span></span>
| <span data-ttu-id="a8fd0-112">类型</span><span class="sxs-lookup"><span data-stu-id="a8fd0-112">Type</span></span> | <span data-ttu-id="a8fd0-113">说明</span><span class="sxs-lookup"><span data-stu-id="a8fd0-113">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="a8fd0-114">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="a8fd0-114">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="a8fd0-115">使用此类型来匹配 Azure Active Directory (Azure AD) 中的现有用户帐户。</span><span class="sxs-lookup"><span data-stu-id="a8fd0-115">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="a8fd0-116">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="a8fd0-116">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="a8fd0-117">使用此类型在 Azure AD 中创建新的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="a8fd0-117">Use this type to create new user accounts in Azure AD.</span></span> |
