---
title: 在 Intune 中管理资源访问证书-Microsoft Graph API
description: 列出管理租户组织的资源访问证书的适用于 Intune 终结点 (REST) 的 Microsoft Graph API。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: d566e570273cfecf213462ab4bf9cea5b76086a9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967530"
---
# <a name="manage-resource-access-certificates-in-intune"></a><span data-ttu-id="7450e-103">在 Intune 中管理资源访问证书</span><span class="sxs-lookup"><span data-stu-id="7450e-103">Manage resource access certificates in Intune</span></span>

> <span data-ttu-id="7450e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7450e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7450e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7450e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7450e-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7450e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7450e-107">您可以使用 Microsoft Graph API 为 Intune 导入 PFX 证书。</span><span class="sxs-lookup"><span data-stu-id="7450e-107">You can import PFX certificates using Microsoft Graph API for Intune.</span></span>

<span data-ttu-id="7450e-108">以下 Graph 资源可用于在 Intune 中管理注册：</span><span class="sxs-lookup"><span data-stu-id="7450e-108">The following Graph resources are available to manage enrollment in Intune:</span></span>

- [<span data-ttu-id="7450e-109">用户 PFX 证书</span><span class="sxs-lookup"><span data-stu-id="7450e-109">User PFX certificate</span></span>](intune-raimportcerts-userpfxcertificate.md)
- [<span data-ttu-id="7450e-110">用户 PFX 预期目的</span><span class="sxs-lookup"><span data-stu-id="7450e-110">User PFX intended purpose</span></span>](intune-raimportcerts-userpfxintendedpurpose.md)
- [<span data-ttu-id="7450e-111">用户 PFX 填充方案</span><span class="sxs-lookup"><span data-stu-id="7450e-111">User PFX padding scheme</span></span>](intune-raimportcerts-userpfxpaddingscheme.md)
