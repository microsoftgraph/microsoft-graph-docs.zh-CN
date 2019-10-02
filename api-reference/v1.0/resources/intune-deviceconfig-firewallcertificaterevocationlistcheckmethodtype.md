---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: FirewallCertificateRevocationListCheckMethod 的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 42f470d7f3d8ef29a69ba8f1cd4f76ddc0f77e96
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359269"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="b4e39-103">firewallCertificateRevocationListCheckMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b4e39-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="b4e39-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b4e39-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4e39-105">FirewallCertificateRevocationListCheckMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="b4e39-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="b4e39-106">成员</span><span class="sxs-lookup"><span data-stu-id="b4e39-106">Members</span></span>
|<span data-ttu-id="b4e39-107">成员</span><span class="sxs-lookup"><span data-stu-id="b4e39-107">Member</span></span>|<span data-ttu-id="b4e39-108">值</span><span class="sxs-lookup"><span data-stu-id="b4e39-108">Value</span></span>|<span data-ttu-id="b4e39-109">说明</span><span class="sxs-lookup"><span data-stu-id="b4e39-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4e39-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b4e39-110">deviceDefault</span></span>|<span data-ttu-id="b4e39-111">0</span><span class="sxs-lookup"><span data-stu-id="b4e39-111">0</span></span>|<span data-ttu-id="b4e39-112">没有由 Intune 配置的值，请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="b4e39-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="b4e39-113">无</span><span class="sxs-lookup"><span data-stu-id="b4e39-113">none</span></span>|<span data-ttu-id="b4e39-114">1</span><span class="sxs-lookup"><span data-stu-id="b4e39-114">1</span></span>|<span data-ttu-id="b4e39-115">不检查证书吊销列表</span><span class="sxs-lookup"><span data-stu-id="b4e39-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="b4e39-116">应试</span><span class="sxs-lookup"><span data-stu-id="b4e39-116">attempt</span></span>|<span data-ttu-id="b4e39-117">双面</span><span class="sxs-lookup"><span data-stu-id="b4e39-117">2</span></span>|<span data-ttu-id="b4e39-118">仅当支票确认证书时，才尝试 CRL 检查并允许证书</span><span class="sxs-lookup"><span data-stu-id="b4e39-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="b4e39-119">无须</span><span class="sxs-lookup"><span data-stu-id="b4e39-119">require</span></span>|<span data-ttu-id="b4e39-120">第三章</span><span class="sxs-lookup"><span data-stu-id="b4e39-120">3</span></span>|<span data-ttu-id="b4e39-121">在允许证书之前，需要进行成功的 CRL 检查</span><span class="sxs-lookup"><span data-stu-id="b4e39-121">Require a successful CRL check before allowing a certificate</span></span>|




