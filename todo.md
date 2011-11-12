- logging
	* WebTarget
	* ProfileTarget
	* Toolbar ?
- base
	* error/exception handling
	  * Convert all PHP errors into exceptions, remove YII_ENABLE_ERROR_HANDLER and error handler (?)
	* module
	* application
	* http exception
	* security
- validators
	* type conversion rules
	* CompareValidator::clientValidateAttribute(): search for "CHtml::activeId"
	* FileValidator, UniqueValidator, ExistValidator, DateValidator: TBD
	* consider merging UniqueValidator and ExistValidator and using a NOT property.
- console command support
- built-in console commands
	+ api doc builder
		* support for markdown syntax
		* support for [[name]]
		* consider to be released as a separate tool for user app docs
- caching
	* a way to invalidate/clear cached data
	* a command to clear cached data
- db
	* DAO
	* schema
	  * write a guide on creating own schema definitions
	* AR
	  * saving related records
	  * collection support for results
	* document-based (should allow storage-specific methods additionally to generic ones)
	  * mongodb
	* key-value-based (should allow storage-specific methods additionally to generic ones)
	  * redis
	  * memcachedb
- i18n
	* consider using PHP built-in support and data
	* message translations, choice format
	* formatting: number and date
	* parsing??
	* make dates/date patterns uniform application-wide including JUI, formats etc.
- helpers
	* array
	* image
	* string
	* file
- web: TBD
	* get/setFlash() should be moved to session component
	* support optional parameter in URL patterns
- gii
    * move generation API out of gii, provide yiic commands to use it. Use same templates for gii/yiic.
	* i18n variant of templates
	* allow to generate module-specific CRUD
- markup and HTML helpers
    * use HTML5 instead of XHTML
- assets
    * ability to manage scripts order (store these in a vector?)
	* http://ryanbigg.com/guides/asset_pipeline.html, http://guides.rubyonrails.org/asset_pipeline.html, use content hash instead of mtime + directory hash.
- collections
    * http://code.google.com/p/yii/source/detail?r=3428
- Requirement checker