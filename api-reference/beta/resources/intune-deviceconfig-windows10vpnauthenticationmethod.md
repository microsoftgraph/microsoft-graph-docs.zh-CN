---
title: windows10VpnAuthenticationMethod 枚举类型
description: Windows 10 VPN 连接类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30b15cf1c03bf44045189938152b83cfb929526b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801601"
---
# <a name="windows10vpnauthenticationmethod-enum-type"></a><span data-ttu-id="fc880-103">windows10VpnAuthenticationMethod 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fc880-103">windows10VpnAuthenticationMethod enum type</span></span>

> <span data-ttu-id="fc880-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fc880-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc880-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc880-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc880-106">Windows 10 VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="fc880-106">Windows 10 VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="fc880-107">成员</span><span class="sxs-lookup"><span data-stu-id="fc880-107">Members</span></span>
|<span data-ttu-id="fc880-108">成员</span><span class="sxs-lookup"><span data-stu-id="fc880-108">Member</span></span>|<span data-ttu-id="fc880-109">值</span><span class="sxs-lookup"><span data-stu-id="fc880-109">Value</span></span>|<span data-ttu-id="fc880-110">说明</span><span class="sxs-lookup"><span data-stu-id="fc880-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc880-111">证书</span><span class="sxs-lookup"><span data-stu-id="fc880-111">certificate</span></span>|<span data-ttu-id="fc880-112">0</span><span class="sxs-lookup"><span data-stu-id="fc880-112">0</span></span>|<span data-ttu-id="fc880-113">使用证书进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="fc880-113">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="fc880-114">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="fc880-114">usernameAndPassword</span></span>|<span data-ttu-id="fc880-115">1</span><span class="sxs-lookup"><span data-stu-id="fc880-115">1</span></span>|<span data-ttu-id="fc880-116">使用用户名和密码进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="fc880-116">Use username and password for authentication.</span></span>|
|<span data-ttu-id="fc880-117">customEapXml</span><span class="sxs-lookup"><span data-stu-id="fc880-117">customEapXml</span></span>|<span data-ttu-id="fc880-118">双面</span><span class="sxs-lookup"><span data-stu-id="fc880-118">2</span></span>|<span data-ttu-id="fc880-119">在自定义 EAP XML 中指定身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="fc880-119">Authentication method is specified in custom EAP XML.</span></span>|





