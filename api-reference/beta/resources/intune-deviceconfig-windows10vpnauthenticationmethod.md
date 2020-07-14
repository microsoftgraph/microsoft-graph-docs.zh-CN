---
title: windows10VpnAuthenticationMethod 枚举类型
description: Windows 10 VPN 连接类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b38ffba54a45bc573e7c6031a6e5aa2aa31d9e49
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124140"
---
# <a name="windows10vpnauthenticationmethod-enum-type"></a><span data-ttu-id="67747-103">windows10VpnAuthenticationMethod 枚举类型</span><span class="sxs-lookup"><span data-stu-id="67747-103">windows10VpnAuthenticationMethod enum type</span></span>

<span data-ttu-id="67747-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67747-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67747-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="67747-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67747-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="67747-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67747-107">Windows 10 VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="67747-107">Windows 10 VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="67747-108">成员</span><span class="sxs-lookup"><span data-stu-id="67747-108">Members</span></span>
|<span data-ttu-id="67747-109">成员</span><span class="sxs-lookup"><span data-stu-id="67747-109">Member</span></span>|<span data-ttu-id="67747-110">值</span><span class="sxs-lookup"><span data-stu-id="67747-110">Value</span></span>|<span data-ttu-id="67747-111">说明</span><span class="sxs-lookup"><span data-stu-id="67747-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67747-112">证书</span><span class="sxs-lookup"><span data-stu-id="67747-112">certificate</span></span>|<span data-ttu-id="67747-113">0</span><span class="sxs-lookup"><span data-stu-id="67747-113">0</span></span>|<span data-ttu-id="67747-114">使用证书进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="67747-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="67747-115">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="67747-115">usernameAndPassword</span></span>|<span data-ttu-id="67747-116">1 </span><span class="sxs-lookup"><span data-stu-id="67747-116">1</span></span>|<span data-ttu-id="67747-117">使用用户名和密码进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="67747-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="67747-118">customEapXml</span><span class="sxs-lookup"><span data-stu-id="67747-118">customEapXml</span></span>|<span data-ttu-id="67747-119">2 </span><span class="sxs-lookup"><span data-stu-id="67747-119">2</span></span>|<span data-ttu-id="67747-120">在自定义 EAP XML 中指定身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="67747-120">Authentication method is specified in custom EAP XML.</span></span>|
|<span data-ttu-id="67747-121">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="67747-121">derivedCredential</span></span>|<span data-ttu-id="67747-122">3 </span><span class="sxs-lookup"><span data-stu-id="67747-122">3</span></span>|<span data-ttu-id="67747-123">使用派生的凭据进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="67747-123">Use Derived Credential for authentication.</span></span>|



