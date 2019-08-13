---
title: managedDevice 资源类型
description: 通过 Intune 托管或预注册的设备
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ca9e4b4e3af7a7f307dd91bce748a7175ac2cce6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372291"
---
# <a name="manageddevice-resource-type"></a><span data-ttu-id="65744-103">managedDevice 资源类型</span><span class="sxs-lookup"><span data-stu-id="65744-103">managedDevice resource type</span></span>

> <span data-ttu-id="65744-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="65744-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65744-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65744-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65744-106">通过 Intune 托管或预注册的设备</span><span class="sxs-lookup"><span data-stu-id="65744-106">Devices that are managed or pre-enrolled through Intune</span></span>

## <a name="methods"></a><span data-ttu-id="65744-107">方法</span><span class="sxs-lookup"><span data-stu-id="65744-107">Methods</span></span>
|<span data-ttu-id="65744-108">方法</span><span class="sxs-lookup"><span data-stu-id="65744-108">Method</span></span>|<span data-ttu-id="65744-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="65744-109">Return Type</span></span>|<span data-ttu-id="65744-110">说明</span><span class="sxs-lookup"><span data-stu-id="65744-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="65744-111">Get managedDevice</span><span class="sxs-lookup"><span data-stu-id="65744-111">Get managedDevice</span></span>](../api/intune-devices-manageddevice-get.md)|[<span data-ttu-id="65744-112">managedDevice</span><span class="sxs-lookup"><span data-stu-id="65744-112">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="65744-113">读取 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="65744-113">Read properties and relationships of the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="65744-114">Update managedDevice</span><span class="sxs-lookup"><span data-stu-id="65744-114">Update managedDevice</span></span>](../api/intune-devices-manageddevice-update.md)|[<span data-ttu-id="65744-115">managedDevice</span><span class="sxs-lookup"><span data-stu-id="65744-115">managedDevice</span></span>](../resources/intune-devices-manageddevice.md)|<span data-ttu-id="65744-116">更新 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="65744-116">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>|
|[<span data-ttu-id="65744-117">executeAction 操作</span><span class="sxs-lookup"><span data-stu-id="65744-117">executeAction action</span></span>](../api/intune-devices-manageddevice-executeaction.md)|[<span data-ttu-id="65744-118">bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="65744-118">bulkManagedDeviceActionResult</span></span>](../resources/intune-devices-bulkmanageddeviceactionresult.md)|<span data-ttu-id="65744-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="65744-119">Not yet documented</span></span>|
|[<span data-ttu-id="65744-120">enableLostMode 操作</span><span class="sxs-lookup"><span data-stu-id="65744-120">enableLostMode action</span></span>](../api/intune-devices-manageddevice-enablelostmode.md)|<span data-ttu-id="65744-121">无</span><span class="sxs-lookup"><span data-stu-id="65744-121">None</span></span>|<span data-ttu-id="65744-122">启用丢失模式</span><span class="sxs-lookup"><span data-stu-id="65744-122">Enable lost mode</span></span>|
|[<span data-ttu-id="65744-123">playLostModeSound 操作</span><span class="sxs-lookup"><span data-stu-id="65744-123">playLostModeSound action</span></span>](../api/intune-devices-manageddevice-playlostmodesound.md)|<span data-ttu-id="65744-124">无</span><span class="sxs-lookup"><span data-stu-id="65744-124">None</span></span>|<span data-ttu-id="65744-125">远程锁定</span><span class="sxs-lookup"><span data-stu-id="65744-125">Remote lock</span></span>|
|[<span data-ttu-id="65744-126">setDeviceName 操作</span><span class="sxs-lookup"><span data-stu-id="65744-126">setDeviceName action</span></span>](../api/intune-devices-manageddevice-setdevicename.md)|<span data-ttu-id="65744-127">无</span><span class="sxs-lookup"><span data-stu-id="65744-127">None</span></span>|<span data-ttu-id="65744-128">设置设备的设备名称。</span><span class="sxs-lookup"><span data-stu-id="65744-128">Set device name of the device.</span></span>|
|[<span data-ttu-id="65744-129">rotateFileVaultKey 操作</span><span class="sxs-lookup"><span data-stu-id="65744-129">rotateFileVaultKey action</span></span>](../api/intune-devices-manageddevice-rotatefilevaultkey.md)|<span data-ttu-id="65744-130">无</span><span class="sxs-lookup"><span data-stu-id="65744-130">None</span></span>|<span data-ttu-id="65744-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="65744-131">Not yet documented</span></span>|
|[<span data-ttu-id="65744-132">getFileVaultKey 函数</span><span class="sxs-lookup"><span data-stu-id="65744-132">getFileVaultKey function</span></span>](../api/intune-devices-manageddevice-getfilevaultkey.md)|<span data-ttu-id="65744-133">字符串</span><span class="sxs-lookup"><span data-stu-id="65744-133">String</span></span>|<span data-ttu-id="65744-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="65744-134">Not yet documented</span></span>|
|[<span data-ttu-id="65744-135">retire 操作</span><span class="sxs-lookup"><span data-stu-id="65744-135">retire action</span></span>](../api/intune-devices-manageddevice-retire.md)|<span data-ttu-id="65744-136">无</span><span class="sxs-lookup"><span data-stu-id="65744-136">None</span></span>|<span data-ttu-id="65744-137">停用设备</span><span class="sxs-lookup"><span data-stu-id="65744-137">Retire a device</span></span>|
|[<span data-ttu-id="65744-138">wipe 操作</span><span class="sxs-lookup"><span data-stu-id="65744-138">wipe action</span></span>](../api/intune-devices-manageddevice-wipe.md)|<span data-ttu-id="65744-139">无</span><span class="sxs-lookup"><span data-stu-id="65744-139">None</span></span>|<span data-ttu-id="65744-140">擦除设备</span><span class="sxs-lookup"><span data-stu-id="65744-140">Wipe a device</span></span>|
|[<span data-ttu-id="65744-141">resetPasscode 操作</span><span class="sxs-lookup"><span data-stu-id="65744-141">resetPasscode action</span></span>](../api/intune-devices-manageddevice-resetpasscode.md)|<span data-ttu-id="65744-142">无</span><span class="sxs-lookup"><span data-stu-id="65744-142">None</span></span>|<span data-ttu-id="65744-143">重置密码</span><span class="sxs-lookup"><span data-stu-id="65744-143">Reset passcode</span></span>|
|[<span data-ttu-id="65744-144">remoteLock 操作</span><span class="sxs-lookup"><span data-stu-id="65744-144">remoteLock action</span></span>](../api/intune-devices-manageddevice-remotelock.md)|<span data-ttu-id="65744-145">无</span><span class="sxs-lookup"><span data-stu-id="65744-145">None</span></span>|<span data-ttu-id="65744-146">远程锁定</span><span class="sxs-lookup"><span data-stu-id="65744-146">Remote lock</span></span>|
|[<span data-ttu-id="65744-147">requestRemoteAssistance 操作</span><span class="sxs-lookup"><span data-stu-id="65744-147">requestRemoteAssistance action</span></span>](../api/intune-devices-manageddevice-requestremoteassistance.md)|<span data-ttu-id="65744-148">无</span><span class="sxs-lookup"><span data-stu-id="65744-148">None</span></span>|<span data-ttu-id="65744-149">请求远程协助</span><span class="sxs-lookup"><span data-stu-id="65744-149">Request remote assistance</span></span>|
|[<span data-ttu-id="65744-150">disableLostMode 操作</span><span class="sxs-lookup"><span data-stu-id="65744-150">disableLostMode action</span></span>](../api/intune-devices-manageddevice-disablelostmode.md)|<span data-ttu-id="65744-151">无</span><span class="sxs-lookup"><span data-stu-id="65744-151">None</span></span>|<span data-ttu-id="65744-152">禁用丢失模式</span><span class="sxs-lookup"><span data-stu-id="65744-152">Disable lost mode</span></span>|
|[<span data-ttu-id="65744-153">locateDevice 操作</span><span class="sxs-lookup"><span data-stu-id="65744-153">locateDevice action</span></span>](../api/intune-devices-manageddevice-locatedevice.md)|<span data-ttu-id="65744-154">无</span><span class="sxs-lookup"><span data-stu-id="65744-154">None</span></span>|<span data-ttu-id="65744-155">查找设备</span><span class="sxs-lookup"><span data-stu-id="65744-155">Locate a device</span></span>|
|[<span data-ttu-id="65744-156">bypassActivationLock 操作</span><span class="sxs-lookup"><span data-stu-id="65744-156">bypassActivationLock action</span></span>](../api/intune-devices-manageddevice-bypassactivationlock.md)|<span data-ttu-id="65744-157">无</span><span class="sxs-lookup"><span data-stu-id="65744-157">None</span></span>|<span data-ttu-id="65744-158">跳过激活锁</span><span class="sxs-lookup"><span data-stu-id="65744-158">Bypass activation lock</span></span>|
|[<span data-ttu-id="65744-159">rebootNow 操作</span><span class="sxs-lookup"><span data-stu-id="65744-159">rebootNow action</span></span>](../api/intune-devices-manageddevice-rebootnow.md)|<span data-ttu-id="65744-160">无</span><span class="sxs-lookup"><span data-stu-id="65744-160">None</span></span>|<span data-ttu-id="65744-161">重新启动设备</span><span class="sxs-lookup"><span data-stu-id="65744-161">Reboot device</span></span>|
|[<span data-ttu-id="65744-162">shutDown 操作</span><span class="sxs-lookup"><span data-stu-id="65744-162">shutDown action</span></span>](../api/intune-devices-manageddevice-shutdown.md)|<span data-ttu-id="65744-163">无</span><span class="sxs-lookup"><span data-stu-id="65744-163">None</span></span>|<span data-ttu-id="65744-164">关闭设备</span><span class="sxs-lookup"><span data-stu-id="65744-164">Shut down device</span></span>|
|[<span data-ttu-id="65744-165">recoverPasscode 操作</span><span class="sxs-lookup"><span data-stu-id="65744-165">recoverPasscode action</span></span>](../api/intune-devices-manageddevice-recoverpasscode.md)|<span data-ttu-id="65744-166">无</span><span class="sxs-lookup"><span data-stu-id="65744-166">None</span></span>|<span data-ttu-id="65744-167">恢复密码</span><span class="sxs-lookup"><span data-stu-id="65744-167">Recover passcode</span></span>|
|[<span data-ttu-id="65744-168">cleanWindowsDevice 操作</span><span class="sxs-lookup"><span data-stu-id="65744-168">cleanWindowsDevice action</span></span>](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|<span data-ttu-id="65744-169">无</span><span class="sxs-lookup"><span data-stu-id="65744-169">None</span></span>|<span data-ttu-id="65744-170">干净的 Windows 设备</span><span class="sxs-lookup"><span data-stu-id="65744-170">Clean Windows device</span></span>|
|[<span data-ttu-id="65744-171">logoutSharedAppleDeviceActiveUser 操作</span><span class="sxs-lookup"><span data-stu-id="65744-171">logoutSharedAppleDeviceActiveUser action</span></span>](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|<span data-ttu-id="65744-172">无</span><span class="sxs-lookup"><span data-stu-id="65744-172">None</span></span>|<span data-ttu-id="65744-173">注销共享 Apple 设备活动用户</span><span class="sxs-lookup"><span data-stu-id="65744-173">Logout shared Apple device active user</span></span>|
|[<span data-ttu-id="65744-174">deleteUserFromSharedAppleDevice 操作</span><span class="sxs-lookup"><span data-stu-id="65744-174">deleteUserFromSharedAppleDevice action</span></span>](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|<span data-ttu-id="65744-175">无</span><span class="sxs-lookup"><span data-stu-id="65744-175">None</span></span>|<span data-ttu-id="65744-176">从共享 Apple 设备中删除用户</span><span class="sxs-lookup"><span data-stu-id="65744-176">Delete user from shared Apple device</span></span>|
|[<span data-ttu-id="65744-177">syncDevice 操作</span><span class="sxs-lookup"><span data-stu-id="65744-177">syncDevice action</span></span>](../api/intune-devices-manageddevice-syncdevice.md)|<span data-ttu-id="65744-178">无</span><span class="sxs-lookup"><span data-stu-id="65744-178">None</span></span>|<span data-ttu-id="65744-179">尚未记录</span><span class="sxs-lookup"><span data-stu-id="65744-179">Not yet documented</span></span>|
|[<span data-ttu-id="65744-180">windowsDefenderScan 操作</span><span class="sxs-lookup"><span data-stu-id="65744-180">windowsDefenderScan action</span></span>](../api/intune-devices-manageddevice-windowsdefenderscan.md)|<span data-ttu-id="65744-181">无</span><span class="sxs-lookup"><span data-stu-id="65744-181">None</span></span>|<span data-ttu-id="65744-182">尚未记录</span><span class="sxs-lookup"><span data-stu-id="65744-182">Not yet documented</span></span>|
|[<span data-ttu-id="65744-183">windowsDefenderUpdateSignatures 操作</span><span class="sxs-lookup"><span data-stu-id="65744-183">windowsDefenderUpdateSignatures action</span></span>](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|<span data-ttu-id="65744-184">无</span><span class="sxs-lookup"><span data-stu-id="65744-184">None</span></span>|<span data-ttu-id="65744-185">尚未记录</span><span class="sxs-lookup"><span data-stu-id="65744-185">Not yet documented</span></span>|
|[<span data-ttu-id="65744-186">updateWindowsDeviceAccount 操作</span><span class="sxs-lookup"><span data-stu-id="65744-186">updateWindowsDeviceAccount action</span></span>](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|<span data-ttu-id="65744-187">无</span><span class="sxs-lookup"><span data-stu-id="65744-187">None</span></span>|<span data-ttu-id="65744-188">尚未记录</span><span class="sxs-lookup"><span data-stu-id="65744-188">Not yet documented</span></span>|
|[<span data-ttu-id="65744-189">revokeAppleVppLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="65744-189">revokeAppleVppLicenses action</span></span>](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|<span data-ttu-id="65744-190">无</span><span class="sxs-lookup"><span data-stu-id="65744-190">None</span></span>|<span data-ttu-id="65744-191">吊销设备的所有 Apple Vpp 许可证</span><span class="sxs-lookup"><span data-stu-id="65744-191">Revoke all Apple Vpp licenses for a device</span></span>|
|[<span data-ttu-id="65744-192">sendCustomNotificationToCompanyPortal 操作</span><span class="sxs-lookup"><span data-stu-id="65744-192">sendCustomNotificationToCompanyPortal action</span></span>](../api/intune-devices-manageddevice-sendcustomnotificationtocompanyportal.md)|<span data-ttu-id="65744-193">无</span><span class="sxs-lookup"><span data-stu-id="65744-193">None</span></span>|<span data-ttu-id="65744-194">尚未记录</span><span class="sxs-lookup"><span data-stu-id="65744-194">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="65744-195">属性</span><span class="sxs-lookup"><span data-stu-id="65744-195">Properties</span></span>
|<span data-ttu-id="65744-196">属性</span><span class="sxs-lookup"><span data-stu-id="65744-196">Property</span></span>|<span data-ttu-id="65744-197">类型</span><span class="sxs-lookup"><span data-stu-id="65744-197">Type</span></span>|<span data-ttu-id="65744-198">说明</span><span class="sxs-lookup"><span data-stu-id="65744-198">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65744-199">id</span><span class="sxs-lookup"><span data-stu-id="65744-199">id</span></span>|<span data-ttu-id="65744-200">String</span><span class="sxs-lookup"><span data-stu-id="65744-200">String</span></span>|<span data-ttu-id="65744-201">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="65744-201">Unique Identifier for the device</span></span>|
|<span data-ttu-id="65744-202">userId</span><span class="sxs-lookup"><span data-stu-id="65744-202">userId</span></span>|<span data-ttu-id="65744-203">String</span><span class="sxs-lookup"><span data-stu-id="65744-203">String</span></span>|<span data-ttu-id="65744-204">与设备关联的用户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="65744-204">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="65744-205">deviceName</span><span class="sxs-lookup"><span data-stu-id="65744-205">deviceName</span></span>|<span data-ttu-id="65744-206">String</span><span class="sxs-lookup"><span data-stu-id="65744-206">String</span></span>|<span data-ttu-id="65744-207">设备的名称</span><span class="sxs-lookup"><span data-stu-id="65744-207">Name of the device</span></span>|
|<span data-ttu-id="65744-208">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="65744-208">hardwareInformation</span></span>|[<span data-ttu-id="65744-209">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="65744-209">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="65744-210">设备的 hardward 详细信息。</span><span class="sxs-lookup"><span data-stu-id="65744-210">The hardward details for the device.</span></span>  <span data-ttu-id="65744-211">包括存储空间、制造商、序列号等信息。</span><span class="sxs-lookup"><span data-stu-id="65744-211">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="65744-212">所有者</span><span class="sxs-lookup"><span data-stu-id="65744-212">ownerType</span></span>|[<span data-ttu-id="65744-213">所有者</span><span class="sxs-lookup"><span data-stu-id="65744-213">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="65744-214">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="65744-214">Ownership of the device.</span></span> <span data-ttu-id="65744-215">可以是 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="65744-215">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="65744-216">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="65744-216">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="65744-217">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="65744-217">managedDeviceOwnerType</span></span>|[<span data-ttu-id="65744-218">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="65744-218">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="65744-219">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="65744-219">Ownership of the device.</span></span> <span data-ttu-id="65744-220">可以是 "公司" 或 "个人"。</span><span class="sxs-lookup"><span data-stu-id="65744-220">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="65744-221">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="65744-221">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="65744-222">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="65744-222">deviceActionResults</span></span>|<span data-ttu-id="65744-223">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="65744-223">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="65744-224">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="65744-224">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="65744-225">managementState</span><span class="sxs-lookup"><span data-stu-id="65744-225">managementState</span></span>|[<span data-ttu-id="65744-226">managementState</span><span class="sxs-lookup"><span data-stu-id="65744-226">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="65744-227">设备的管理状态。</span><span class="sxs-lookup"><span data-stu-id="65744-227">Management state of the device.</span></span> <span data-ttu-id="65744-228">可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。</span><span class="sxs-lookup"><span data-stu-id="65744-228">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="65744-229">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="65744-229">enrolledDateTime</span></span>|<span data-ttu-id="65744-230">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65744-230">DateTimeOffset</span></span>|<span data-ttu-id="65744-231">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="65744-231">Enrollment time of the device.</span></span>|
|<span data-ttu-id="65744-232">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="65744-232">lastSyncDateTime</span></span>|<span data-ttu-id="65744-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65744-233">DateTimeOffset</span></span>|<span data-ttu-id="65744-234">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="65744-234">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="65744-235">chassisType</span><span class="sxs-lookup"><span data-stu-id="65744-235">chassisType</span></span>|[<span data-ttu-id="65744-236">chassisType</span><span class="sxs-lookup"><span data-stu-id="65744-236">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="65744-237">设备的机箱类型。</span><span class="sxs-lookup"><span data-stu-id="65744-237">Chassis type of the device.</span></span> <span data-ttu-id="65744-238">可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。</span><span class="sxs-lookup"><span data-stu-id="65744-238">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="65744-239">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="65744-239">operatingSystem</span></span>|<span data-ttu-id="65744-240">String</span><span class="sxs-lookup"><span data-stu-id="65744-240">String</span></span>|<span data-ttu-id="65744-241">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="65744-241">Operating system of the device.</span></span> <span data-ttu-id="65744-242">Windows、iOS 等。</span><span class="sxs-lookup"><span data-stu-id="65744-242">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="65744-243">deviceType</span><span class="sxs-lookup"><span data-stu-id="65744-243">deviceType</span></span>|[<span data-ttu-id="65744-244">deviceType</span><span class="sxs-lookup"><span data-stu-id="65744-244">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="65744-245">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="65744-245">Platform of the device.</span></span> <span data-ttu-id="65744-246">可能的值为`desktop`: `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer`、、、、、、、、、、、、、、、、 `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="65744-246">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="65744-247">complianceState</span><span class="sxs-lookup"><span data-stu-id="65744-247">complianceState</span></span>|[<span data-ttu-id="65744-248">complianceState</span><span class="sxs-lookup"><span data-stu-id="65744-248">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="65744-249">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="65744-249">Compliance state of the device.</span></span> <span data-ttu-id="65744-250">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="65744-250">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="65744-251">jailBroken</span><span class="sxs-lookup"><span data-stu-id="65744-251">jailBroken</span></span>|<span data-ttu-id="65744-252">String</span><span class="sxs-lookup"><span data-stu-id="65744-252">String</span></span>|<span data-ttu-id="65744-253">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="65744-253">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="65744-254">managementAgent</span><span class="sxs-lookup"><span data-stu-id="65744-254">managementAgent</span></span>|[<span data-ttu-id="65744-255">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="65744-255">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="65744-256">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="65744-256">Management channel of the device.</span></span> <span data-ttu-id="65744-257">Intune、EAS 等。可能的值为`eas`: `mdm`、 `easMdm`、 `intuneClient` `easIntuneClient` `configurationManagerClient` `configurationManagerClientMdm` `configurationManagerClientMdmEas` `unknown`、、、、、、、、 `microsoft365ManagedMdm` `jamf` `googleCloudDevicePolicyController`</span><span class="sxs-lookup"><span data-stu-id="65744-257">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="65744-258">osVersion</span><span class="sxs-lookup"><span data-stu-id="65744-258">osVersion</span></span>|<span data-ttu-id="65744-259">String</span><span class="sxs-lookup"><span data-stu-id="65744-259">String</span></span>|<span data-ttu-id="65744-260">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="65744-260">Operating system version of the device.</span></span>|
|<span data-ttu-id="65744-261">easActivated</span><span class="sxs-lookup"><span data-stu-id="65744-261">easActivated</span></span>|<span data-ttu-id="65744-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="65744-262">Boolean</span></span>|<span data-ttu-id="65744-263">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="65744-263">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="65744-264">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="65744-264">easDeviceId</span></span>|<span data-ttu-id="65744-265">String</span><span class="sxs-lookup"><span data-stu-id="65744-265">String</span></span>|<span data-ttu-id="65744-266">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="65744-266">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="65744-267">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="65744-267">easActivationDateTime</span></span>|<span data-ttu-id="65744-268">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65744-268">DateTimeOffset</span></span>|<span data-ttu-id="65744-269">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="65744-269">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="65744-270">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="65744-270">aadRegistered</span></span>|<span data-ttu-id="65744-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="65744-271">Boolean</span></span>|<span data-ttu-id="65744-272">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="65744-272">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="65744-273">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="65744-273">azureADRegistered</span></span>|<span data-ttu-id="65744-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="65744-274">Boolean</span></span>|<span data-ttu-id="65744-275">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="65744-275">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="65744-276">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="65744-276">deviceEnrollmentType</span></span>|[<span data-ttu-id="65744-277">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="65744-277">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="65744-278">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="65744-278">Enrollment type of the device.</span></span> <span data-ttu-id="65744-279">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="65744-279">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="65744-280">lostModeState</span><span class="sxs-lookup"><span data-stu-id="65744-280">lostModeState</span></span>|[<span data-ttu-id="65744-281">lostModeState</span><span class="sxs-lookup"><span data-stu-id="65744-281">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="65744-282">指示是否已启用或禁用了丢失模式。</span><span class="sxs-lookup"><span data-stu-id="65744-282">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="65744-283">可取值为：`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="65744-283">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="65744-284">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="65744-284">activationLockBypassCode</span></span>|<span data-ttu-id="65744-285">String</span><span class="sxs-lookup"><span data-stu-id="65744-285">String</span></span>|<span data-ttu-id="65744-286">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="65744-286">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="65744-287">emailAddress</span><span class="sxs-lookup"><span data-stu-id="65744-287">emailAddress</span></span>|<span data-ttu-id="65744-288">String</span><span class="sxs-lookup"><span data-stu-id="65744-288">String</span></span>|<span data-ttu-id="65744-289">与设备关联的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="65744-289">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="65744-290">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="65744-290">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="65744-291">String</span><span class="sxs-lookup"><span data-stu-id="65744-291">String</span></span>|<span data-ttu-id="65744-292">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="65744-292">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="65744-293">只读。</span><span class="sxs-lookup"><span data-stu-id="65744-293">Read only.</span></span>|
|<span data-ttu-id="65744-294">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="65744-294">azureADDeviceId</span></span>|<span data-ttu-id="65744-295">String</span><span class="sxs-lookup"><span data-stu-id="65744-295">String</span></span>|<span data-ttu-id="65744-296">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="65744-296">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="65744-297">只读。</span><span class="sxs-lookup"><span data-stu-id="65744-297">Read only.</span></span>|
|<span data-ttu-id="65744-298">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="65744-298">deviceRegistrationState</span></span>|[<span data-ttu-id="65744-299">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="65744-299">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="65744-300">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="65744-300">Device registration state.</span></span> <span data-ttu-id="65744-301">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="65744-301">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="65744-302">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="65744-302">deviceCategoryDisplayName</span></span>|<span data-ttu-id="65744-303">String</span><span class="sxs-lookup"><span data-stu-id="65744-303">String</span></span>|<span data-ttu-id="65744-304">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="65744-304">Device category display name</span></span>|
|<span data-ttu-id="65744-305">isSupervised</span><span class="sxs-lookup"><span data-stu-id="65744-305">isSupervised</span></span>|<span data-ttu-id="65744-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="65744-306">Boolean</span></span>|<span data-ttu-id="65744-307">设备受监督状态</span><span class="sxs-lookup"><span data-stu-id="65744-307">Device supervised status</span></span>|
|<span data-ttu-id="65744-308">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="65744-308">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="65744-309">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65744-309">DateTimeOffset</span></span>|<span data-ttu-id="65744-310">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="65744-310">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="65744-311">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="65744-311">exchangeAccessState</span></span>|[<span data-ttu-id="65744-312">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="65744-312">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="65744-313">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="65744-313">The Access State of the device in Exchange.</span></span> <span data-ttu-id="65744-314">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="65744-314">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="65744-315">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="65744-315">exchangeAccessStateReason</span></span>|[<span data-ttu-id="65744-316">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="65744-316">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="65744-317">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="65744-317">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="65744-318">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="65744-318">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="65744-319">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="65744-319">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="65744-320">String</span><span class="sxs-lookup"><span data-stu-id="65744-320">String</span></span>|<span data-ttu-id="65744-321">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="65744-321">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="65744-322">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="65744-322">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="65744-323">String</span><span class="sxs-lookup"><span data-stu-id="65744-323">String</span></span>|<span data-ttu-id="65744-324">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="65744-324">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="65744-325">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="65744-325">isEncrypted</span></span>|<span data-ttu-id="65744-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="65744-326">Boolean</span></span>|<span data-ttu-id="65744-327">设备加密状态</span><span class="sxs-lookup"><span data-stu-id="65744-327">Device encryption status</span></span>|
|<span data-ttu-id="65744-328">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="65744-328">userPrincipalName</span></span>|<span data-ttu-id="65744-329">字符串</span><span class="sxs-lookup"><span data-stu-id="65744-329">String</span></span>|<span data-ttu-id="65744-330">设备用户主体名称</span><span class="sxs-lookup"><span data-stu-id="65744-330">Device user principal name</span></span>|
|<span data-ttu-id="65744-331">model</span><span class="sxs-lookup"><span data-stu-id="65744-331">model</span></span>|<span data-ttu-id="65744-332">String</span><span class="sxs-lookup"><span data-stu-id="65744-332">String</span></span>|<span data-ttu-id="65744-333">设备的型号</span><span class="sxs-lookup"><span data-stu-id="65744-333">Model of the device</span></span>|
|<span data-ttu-id="65744-334">manufacturer</span><span class="sxs-lookup"><span data-stu-id="65744-334">manufacturer</span></span>|<span data-ttu-id="65744-335">String</span><span class="sxs-lookup"><span data-stu-id="65744-335">String</span></span>|<span data-ttu-id="65744-336">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="65744-336">Manufacturer of the device</span></span>|
|<span data-ttu-id="65744-337">imei</span><span class="sxs-lookup"><span data-stu-id="65744-337">imei</span></span>|<span data-ttu-id="65744-338">String</span><span class="sxs-lookup"><span data-stu-id="65744-338">String</span></span>|<span data-ttu-id="65744-339">IMEI</span><span class="sxs-lookup"><span data-stu-id="65744-339">IMEI</span></span>|
|<span data-ttu-id="65744-340">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="65744-340">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="65744-341">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65744-341">DateTimeOffset</span></span>|<span data-ttu-id="65744-342">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="65744-342">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="65744-343">serialNumber</span><span class="sxs-lookup"><span data-stu-id="65744-343">serialNumber</span></span>|<span data-ttu-id="65744-344">字符串</span><span class="sxs-lookup"><span data-stu-id="65744-344">String</span></span>|<span data-ttu-id="65744-345">序列号</span><span class="sxs-lookup"><span data-stu-id="65744-345">SerialNumber</span></span>|
|<span data-ttu-id="65744-346">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="65744-346">phoneNumber</span></span>|<span data-ttu-id="65744-347">String</span><span class="sxs-lookup"><span data-stu-id="65744-347">String</span></span>|<span data-ttu-id="65744-348">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="65744-348">Phone number of the device</span></span>|
|<span data-ttu-id="65744-349">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="65744-349">androidSecurityPatchLevel</span></span>|<span data-ttu-id="65744-350">String</span><span class="sxs-lookup"><span data-stu-id="65744-350">String</span></span>|<span data-ttu-id="65744-351">Android 安全修补程序级别</span><span class="sxs-lookup"><span data-stu-id="65744-351">Android security patch level</span></span>|
|<span data-ttu-id="65744-352">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="65744-352">userDisplayName</span></span>|<span data-ttu-id="65744-353">String</span><span class="sxs-lookup"><span data-stu-id="65744-353">String</span></span>|<span data-ttu-id="65744-354">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="65744-354">User display name</span></span>|
|<span data-ttu-id="65744-355">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="65744-355">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="65744-356">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="65744-356">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="65744-357">ConfigrMgr 客户端启用的功能</span><span class="sxs-lookup"><span data-stu-id="65744-357">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="65744-358">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="65744-358">wiFiMacAddress</span></span>|<span data-ttu-id="65744-359">String</span><span class="sxs-lookup"><span data-stu-id="65744-359">String</span></span>|<span data-ttu-id="65744-360">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="65744-360">Wi-Fi MAC</span></span>|
|<span data-ttu-id="65744-361">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="65744-361">deviceHealthAttestationState</span></span>|[<span data-ttu-id="65744-362">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="65744-362">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="65744-363">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="65744-363">The device health attestation state.</span></span>|
|<span data-ttu-id="65744-364">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="65744-364">subscriberCarrier</span></span>|<span data-ttu-id="65744-365">String</span><span class="sxs-lookup"><span data-stu-id="65744-365">String</span></span>|<span data-ttu-id="65744-366">订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="65744-366">Subscriber Carrier</span></span>|
|<span data-ttu-id="65744-367">meid</span><span class="sxs-lookup"><span data-stu-id="65744-367">meid</span></span>|<span data-ttu-id="65744-368">String</span><span class="sxs-lookup"><span data-stu-id="65744-368">String</span></span>|<span data-ttu-id="65744-369">MEID</span><span class="sxs-lookup"><span data-stu-id="65744-369">MEID</span></span>|
|<span data-ttu-id="65744-370">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="65744-370">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="65744-371">Int64</span><span class="sxs-lookup"><span data-stu-id="65744-371">Int64</span></span>|<span data-ttu-id="65744-372">存储空间总字节数</span><span class="sxs-lookup"><span data-stu-id="65744-372">Total Storage in Bytes</span></span>|
|<span data-ttu-id="65744-373">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="65744-373">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="65744-374">Int64</span><span class="sxs-lookup"><span data-stu-id="65744-374">Int64</span></span>|<span data-ttu-id="65744-375">可用存储空间字节数</span><span class="sxs-lookup"><span data-stu-id="65744-375">Free Storage in Bytes</span></span>|
|<span data-ttu-id="65744-376">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="65744-376">managedDeviceName</span></span>|<span data-ttu-id="65744-377">String</span><span class="sxs-lookup"><span data-stu-id="65744-377">String</span></span>|<span data-ttu-id="65744-378">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="65744-378">Automatically generated name to identify a device.</span></span> <span data-ttu-id="65744-379">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="65744-379">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="65744-380">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="65744-380">partnerReportedThreatState</span></span>|[<span data-ttu-id="65744-381">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="65744-381">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="65744-382">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="65744-382">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="65744-383">只读。</span><span class="sxs-lookup"><span data-stu-id="65744-383">Read Only.</span></span> <span data-ttu-id="65744-384">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。</span><span class="sxs-lookup"><span data-stu-id="65744-384">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="65744-385">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="65744-385">retireAfterDateTime</span></span>|<span data-ttu-id="65744-386">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65744-386">DateTimeOffset</span></span>|<span data-ttu-id="65744-387">指示当设备因计划操作而自动停用的时间。</span><span class="sxs-lookup"><span data-stu-id="65744-387">Indicates the time after when a device will be auto retired because of scheduled action.</span></span>|
|<span data-ttu-id="65744-388">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="65744-388">usersLoggedOn</span></span>|<span data-ttu-id="65744-389">[loggedOnUser](../resources/intune-devices-loggedonuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="65744-389">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="65744-390">指示设备的上次登录用户</span><span class="sxs-lookup"><span data-stu-id="65744-390">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="65744-391">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="65744-391">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="65744-392">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65744-392">DateTimeOffset</span></span>|<span data-ttu-id="65744-393">报告设置了 preferMdmOverGroupPolicy 设置的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="65744-393">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="65744-394">设置后, 如果存在冲突, Intune MDM 设置将覆盖组策略设置。</span><span class="sxs-lookup"><span data-stu-id="65744-394">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="65744-395">只读。</span><span class="sxs-lookup"><span data-stu-id="65744-395">Read Only.</span></span>|
|<span data-ttu-id="65744-396">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="65744-396">autopilotEnrolled</span></span>|<span data-ttu-id="65744-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="65744-397">Boolean</span></span>|<span data-ttu-id="65744-398">如果托管设备是通过自动引导注册的, 则报告。</span><span class="sxs-lookup"><span data-stu-id="65744-398">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="65744-399">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="65744-399">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="65744-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="65744-400">Boolean</span></span>|<span data-ttu-id="65744-401">如果托管 iOS 设备是用户审批注册, 则报告。</span><span class="sxs-lookup"><span data-stu-id="65744-401">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="65744-402">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="65744-402">managementCertificateExpirationDate</span></span>|<span data-ttu-id="65744-403">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65744-403">DateTimeOffset</span></span>|<span data-ttu-id="65744-404">报告设备管理证书到期日期</span><span class="sxs-lookup"><span data-stu-id="65744-404">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="65744-405">iccid</span><span class="sxs-lookup"><span data-stu-id="65744-405">iccid</span></span>|<span data-ttu-id="65744-406">String</span><span class="sxs-lookup"><span data-stu-id="65744-406">String</span></span>|<span data-ttu-id="65744-407">集成的电路卡标识符, 它是 SIM 卡的唯一标识号。</span><span class="sxs-lookup"><span data-stu-id="65744-407">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="65744-408">udid</span><span class="sxs-lookup"><span data-stu-id="65744-408">udid</span></span>|<span data-ttu-id="65744-409">String</span><span class="sxs-lookup"><span data-stu-id="65744-409">String</span></span>|<span data-ttu-id="65744-410">IOS 和 macOS 设备的唯一设备标识符。</span><span class="sxs-lookup"><span data-stu-id="65744-410">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="65744-411">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="65744-411">roleScopeTagIds</span></span>|<span data-ttu-id="65744-412">String collection</span><span class="sxs-lookup"><span data-stu-id="65744-412">String collection</span></span>|<span data-ttu-id="65744-413">此设备实例的范围标记 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="65744-413">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="65744-414">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="65744-414">windowsActiveMalwareCount</span></span>|<span data-ttu-id="65744-415">Int32</span><span class="sxs-lookup"><span data-stu-id="65744-415">Int32</span></span>|<span data-ttu-id="65744-416">此 windows 设备的活动恶意软件计数</span><span class="sxs-lookup"><span data-stu-id="65744-416">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="65744-417">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="65744-417">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="65744-418">Int32</span><span class="sxs-lookup"><span data-stu-id="65744-418">Int32</span></span>|<span data-ttu-id="65744-419">此 windows 设备的修正的恶意软件计数</span><span class="sxs-lookup"><span data-stu-id="65744-419">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="65744-420">notes</span><span class="sxs-lookup"><span data-stu-id="65744-420">notes</span></span>|<span data-ttu-id="65744-421">String</span><span class="sxs-lookup"><span data-stu-id="65744-421">String</span></span>|<span data-ttu-id="65744-422">IT 管理员创建的设备上的注释</span><span class="sxs-lookup"><span data-stu-id="65744-422">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="65744-423">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="65744-423">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="65744-424">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="65744-424">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="65744-425">Configuration manager 客户端运行状况状态, 仅对由 MDM/ConfigMgr 代理管理的设备有效</span><span class="sxs-lookup"><span data-stu-id="65744-425">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|
|<span data-ttu-id="65744-426">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="65744-426">configurationManagerClientInformation</span></span>|[<span data-ttu-id="65744-427">configurationManagerClientInformation</span><span class="sxs-lookup"><span data-stu-id="65744-427">configurationManagerClientInformation</span></span>](../resources/intune-devices-configurationmanagerclientinformation.md)|<span data-ttu-id="65744-428">Configuration manager 客户端信息, 仅对受 ConfigMgr 代理管理、duel 管理或三方管理的设备有效</span><span class="sxs-lookup"><span data-stu-id="65744-428">Configuration manager client information, valid only for devices managed, duel-managed or tri-managed by ConfigMgr Agent</span></span>|

## <a name="relationships"></a><span data-ttu-id="65744-429">关系</span><span class="sxs-lookup"><span data-stu-id="65744-429">Relationships</span></span>
|<span data-ttu-id="65744-430">关系</span><span class="sxs-lookup"><span data-stu-id="65744-430">Relationship</span></span>|<span data-ttu-id="65744-431">类型</span><span class="sxs-lookup"><span data-stu-id="65744-431">Type</span></span>|<span data-ttu-id="65744-432">说明</span><span class="sxs-lookup"><span data-stu-id="65744-432">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65744-433">detectedApps</span><span class="sxs-lookup"><span data-stu-id="65744-433">detectedApps</span></span>|<span data-ttu-id="65744-434">[detectedApp](../resources/intune-devices-detectedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="65744-434">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="65744-435">设备上当前安装的所有应用程序</span><span class="sxs-lookup"><span data-stu-id="65744-435">All applications currently installed on the device</span></span>|
|<span data-ttu-id="65744-436">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="65744-436">deviceCategory</span></span>|[<span data-ttu-id="65744-437">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="65744-437">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="65744-438">设备类别</span><span class="sxs-lookup"><span data-stu-id="65744-438">Device category</span></span>|
|<span data-ttu-id="65744-439">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="65744-439">windowsProtectionState</span></span>|[<span data-ttu-id="65744-440">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="65744-440">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="65744-441">设备保护状态。</span><span class="sxs-lookup"><span data-stu-id="65744-441">The device protection status.</span></span>|
|<span data-ttu-id="65744-442">users</span><span class="sxs-lookup"><span data-stu-id="65744-442">users</span></span>|<span data-ttu-id="65744-443">[user](../resources/intune-shared-user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="65744-443">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="65744-444">与托管设备关联的主要用户。</span><span class="sxs-lookup"><span data-stu-id="65744-444">The primary users associated with the managed device.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65744-445">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65744-445">JSON Representation</span></span>
<span data-ttu-id="65744-446">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65744-446">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)",
  "userId": "String",
  "deviceName": "String",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "String",
    "totalStorageSpace": 1024,
    "freeStorageSpace": 1024,
    "imei": "String",
    "meid": "String",
    "manufacturer": "String",
    "model": "String",
    "phoneNumber": "String",
    "subscriberCarrier": "String",
    "cellularTechnology": "String",
    "wifiMac": "String",
    "operatingSystemLanguage": "String",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "String",
        "dataToSync": true,
        "dataQuota": 1024,
        "dataUsed": 1024
      }
    ],
    "tpmSpecificationVersion": "String",
    "operatingSystemEdition": "String",
    "deviceFullQualifiedDomainName": "String",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
    "deviceGuardVirtualizationBasedSecurityState": "String",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "String",
    "osBuildNumber": "String"
  },
  "ownerType": "String",
  "managedDeviceOwnerType": "String",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ],
  "managementState": "String",
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "chassisType": "String",
  "operatingSystem": "String",
  "deviceType": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "lostModeState": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureActiveDirectoryDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceRegistrationState": "String",
  "deviceCategoryDisplayName": "String",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "String (timestamp)",
  "exchangeAccessState": "String",
  "exchangeAccessStateReason": "String",
  "remoteAssistanceSessionUrl": "String",
  "remoteAssistanceSessionErrorDetails": "String",
  "isEncrypted": true,
  "userPrincipalName": "String",
  "model": "String",
  "manufacturer": "String",
  "imei": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "serialNumber": "String",
  "phoneNumber": "String",
  "androidSecurityPatchLevel": "String",
  "userDisplayName": "String",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
  },
  "wiFiMacAddress": "String",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "String",
    "contentNamespaceUrl": "String",
    "deviceHealthAttestationStatus": "String",
    "contentVersion": "String",
    "issuedDateTime": "String (timestamp)",
    "attestationIdentityKey": "String",
    "resetCount": 1024,
    "restartCount": 1024,
    "dataExcutionPolicy": "String",
    "bitLockerStatus": "String",
    "bootManagerVersion": "String",
    "codeIntegrityCheckVersion": "String",
    "secureBoot": "String",
    "bootDebugging": "String",
    "operatingSystemKernelDebugging": "String",
    "codeIntegrity": "String",
    "testSigning": "String",
    "safeMode": "String",
    "windowsPE": "String",
    "earlyLaunchAntiMalwareDriverProtection": "String",
    "virtualSecureMode": "String",
    "pcrHashAlgorithm": "String",
    "bootAppSecurityVersion": "String",
    "bootManagerSecurityVersion": "String",
    "tpmVersion": "String",
    "pcr0": "String",
    "secureBootConfigurationPolicyFingerPrint": "String",
    "codeIntegrityPolicy": "String",
    "bootRevisionListInfo": "String",
    "operatingSystemRevListInfo": "String",
    "healthStatusMismatchInfo": "String",
    "healthAttestationSupportedStatus": "String"
  },
  "subscriberCarrier": "String",
  "meid": "String",
  "totalStorageSpaceInBytes": 1024,
  "freeStorageSpaceInBytes": 1024,
  "managedDeviceName": "String",
  "partnerReportedThreatState": "String",
  "retireAfterDateTime": "String (timestamp)",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "String",
      "lastLogOnDateTime": "String (timestamp)"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "String (timestamp)",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "String (timestamp)",
  "iccid": "String",
  "udid": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "windowsActiveMalwareCount": 1024,
  "windowsRemediatedMalwareCount": 1024,
  "notes": "String",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "String",
    "errorCode": 1024,
    "lastSyncDateTime": "String (timestamp)"
  },
  "configurationManagerClientInformation": {
    "@odata.type": "microsoft.graph.configurationManagerClientInformation",
    "clientIdentifier": "String"
  }
}
```



