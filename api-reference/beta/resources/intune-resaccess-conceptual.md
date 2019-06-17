---
title: 在 Intune 中管理资源访问证书-Microsoft Graph API
description: 列出管理租户组织的资源访问证书的适用于 Intune 终结点 (REST) 的 Microsoft Graph API。
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ed680af82eb041e93cf73cb6ed3c390b989d8bc3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996258"
---
# <a name="manage-resource-access-certificates-in-intune"></a><span data-ttu-id="351b3-103">在 Intune 中管理资源访问证书</span><span class="sxs-lookup"><span data-stu-id="351b3-103">Manage resource access certificates in Intune</span></span>

> <span data-ttu-id="351b3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="351b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="351b3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="351b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="351b3-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="351b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="351b3-107">您可以使用 Microsoft Graph API 为 Intune 导入 PFX 证书。</span><span class="sxs-lookup"><span data-stu-id="351b3-107">You can import PFX certificates using Microsoft Graph API for Intune.</span></span>

<span data-ttu-id="351b3-108">以下 Graph 资源可用于在 Intune 中管理注册：</span><span class="sxs-lookup"><span data-stu-id="351b3-108">The following Graph resources are available to manage enrollment in Intune:</span></span>

- [<span data-ttu-id="351b3-109">用户 PFX 证书</span><span class="sxs-lookup"><span data-stu-id="351b3-109">User PFX certificate</span></span>](intune-raimportcerts-userpfxcertificate.md)
- [<span data-ttu-id="351b3-110">用户 PFX 预期目的</span><span class="sxs-lookup"><span data-stu-id="351b3-110">User PFX intended purpose</span></span>](intune-raimportcerts-userpfxintendedpurpose.md)
- [<span data-ttu-id="351b3-111">用户 PFX 填充方案</span><span class="sxs-lookup"><span data-stu-id="351b3-111">User PFX padding scheme</span></span>](intune-raimportcerts-userpfxpaddingscheme.md)
