---
title: 在 Intune 中管理资源访问证书-Microsoft Graph API
description: 列出管理租户组织的资源访问证书的适用于 Intune 终结点（REST）的 Microsoft Graph API。
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d79e455db0b6112bbd44b12a1614750311d42ca7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527502"
---
# <a name="manage-resource-access-certificates-in-intune"></a><span data-ttu-id="44410-103">在 Intune 中管理资源访问证书</span><span class="sxs-lookup"><span data-stu-id="44410-103">Manage resource access certificates in Intune</span></span>

<span data-ttu-id="44410-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="44410-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44410-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="44410-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44410-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="44410-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44410-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="44410-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44410-108">您可以使用 Microsoft Graph API 为 Intune 导入 PFX 证书。</span><span class="sxs-lookup"><span data-stu-id="44410-108">You can import PFX certificates using Microsoft Graph API for Intune.</span></span>

<span data-ttu-id="44410-109">以下 Graph 资源可用于在 Intune 中管理注册：</span><span class="sxs-lookup"><span data-stu-id="44410-109">The following Graph resources are available to manage enrollment in Intune:</span></span>

- [<span data-ttu-id="44410-110">用户 PFX 证书</span><span class="sxs-lookup"><span data-stu-id="44410-110">User PFX certificate</span></span>](intune-raimportcerts-userpfxcertificate.md)
- [<span data-ttu-id="44410-111">用户 PFX 预期目的</span><span class="sxs-lookup"><span data-stu-id="44410-111">User PFX intended purpose</span></span>](intune-raimportcerts-userpfxintendedpurpose.md)
- [<span data-ttu-id="44410-112">用户 PFX 填充方案</span><span class="sxs-lookup"><span data-stu-id="44410-112">User PFX padding scheme</span></span>](intune-raimportcerts-userpfxpaddingscheme.md)
