---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: FirewallCertificateRevocationListCheckMethod 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4c9a94dc19064fc01d70bfa1123d20fec414eac0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526442"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="058a1-103">firewallCertificateRevocationListCheckMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="058a1-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="058a1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="058a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="058a1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="058a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="058a1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="058a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="058a1-107">FirewallCertificateRevocationListCheckMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="058a1-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="058a1-108">成员</span><span class="sxs-lookup"><span data-stu-id="058a1-108">Members</span></span>
|<span data-ttu-id="058a1-109">成员</span><span class="sxs-lookup"><span data-stu-id="058a1-109">Member</span></span>|<span data-ttu-id="058a1-110">值</span><span class="sxs-lookup"><span data-stu-id="058a1-110">Value</span></span>|<span data-ttu-id="058a1-111">说明</span><span class="sxs-lookup"><span data-stu-id="058a1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="058a1-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="058a1-112">deviceDefault</span></span>|<span data-ttu-id="058a1-113">0</span><span class="sxs-lookup"><span data-stu-id="058a1-113">0</span></span>|<span data-ttu-id="058a1-114">没有由 Intune 配置的值，请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="058a1-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="058a1-115">无</span><span class="sxs-lookup"><span data-stu-id="058a1-115">none</span></span>|<span data-ttu-id="058a1-116">1 </span><span class="sxs-lookup"><span data-stu-id="058a1-116">1</span></span>|<span data-ttu-id="058a1-117">不检查证书吊销列表</span><span class="sxs-lookup"><span data-stu-id="058a1-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="058a1-118">应试</span><span class="sxs-lookup"><span data-stu-id="058a1-118">attempt</span></span>|<span data-ttu-id="058a1-119">2 </span><span class="sxs-lookup"><span data-stu-id="058a1-119">2</span></span>|<span data-ttu-id="058a1-120">仅当支票确认证书时，才尝试 CRL 检查并允许证书</span><span class="sxs-lookup"><span data-stu-id="058a1-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="058a1-121">无须</span><span class="sxs-lookup"><span data-stu-id="058a1-121">require</span></span>|<span data-ttu-id="058a1-122">3 </span><span class="sxs-lookup"><span data-stu-id="058a1-122">3</span></span>|<span data-ttu-id="058a1-123">在允许证书之前，需要进行成功的 CRL 检查</span><span class="sxs-lookup"><span data-stu-id="058a1-123">Require a successful CRL check before allowing a certificate</span></span>|



